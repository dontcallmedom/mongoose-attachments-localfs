## mongoose-attachments-localfs

Simple File System Storage Provider for [mongoose-attachments](https://github.com/firebaseco/mongoose-attachments).

### Installation

    $ npm install mongoose-attachments-localfs

### Usage

The library will register automatically with `mongoose-attachments` by performing `require`:

    require('mongoose-attachments-localfs')


This 'provider' stores the images created via mongoose-attachments in the local file system.
It requires that the option 'directory' points to the absolute path of the directory where it will create subfolders per image type.

Example: type is `thumb` and `directory` points to `/path/to/public/images/`
When storing data into the schema, the thumbnail created by mongoose-attachemnts is stored as `/path/to/public/images/thumb/<ObjectID>-thumb.<format>`.
The absolute path to the image is stored in `Model.image.<type>.path`.

For further instructions check [mongoose-attachments](https://github.com/firebaseco/mongoose-attachments).

### Provider Configuration
#### Provider Name:

    fs


### Contributors

* [Johan Hernandez](https://github.com/thepumpkin1979)
* [Chantal Ackermann](https://github.com/nuarhu)

## License (MIT)

Copyright (c) 2012 IT Agenten - http://www.it-agenten.com

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

