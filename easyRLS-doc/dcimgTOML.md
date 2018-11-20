# Help on how to fill TOML files for dcimg

When you try to read for the first time a dcimg file, the program will generate a 'toml' file beside it which looks like this.

    filename = "rec00001.dcimg"
    [size]
    x = 666
    y = 1024
    z = 8
    t = 2000
    [byte]
    depth = "uint16"
    header = 0
    clock = 0
    endianness = "little"
    [meta]
    space = "----"
    layers = [1, 2, 3, 4, 5, 6, 7, 8]

You have to manually fill certain fields. 

## size
If no image were provided, fill in the **x** and **y** field *as if it were RAS space* (x = size in the left → right direction, y = size in the posterior → anterior direction...).

## byte
For the header and clock fields, see [the doc](https://github.com/LaboJeanPerrin/wiki/blob/master/Format/dcimg.md) on dcimg files. The values of **header** and **clock** depend of your version of HCImage software.

## meta
To fill in the **space** field, please refer to the [RAS guide](https://github.com/LaboJeanPerrin/wiki/blob/master/Format/RAS.md).