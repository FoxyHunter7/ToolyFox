# ToolyFox
An all in one (easy to) self-host toolbox.

> [!NOTE]
> *Development is pending (I'm planning to start this summer, and have a first stable version out before the end of september)*

Below are the features currently planned, feel free to suggest (through feature-request issues) any features or functionality you'd like to see as well :)

- **Conversion**
- Any to any _(batch)_ file conversion.
  - Upload file(s) to convert, a mix of formats allowed, specify the output format, and all files will be converted to that format.
  - Starting with: image, video & PDF
- **Network**
  - Opening the network page shows you some basic, like in a header or status bar information
    - any retrievable through: https://developer.mozilla.org/en-US/docs/Web/API/Navigator/connection
    - public ip
      - The webserver hosting the toolbox will need an endpoint for the frontend to request with what IP it contacted the server
      - Documentation will clearly need to state that when accessing over a local network, (with eg. local dns setup) you will see your local ip not public ip.)
      - Make this configurable in the settings, if we should use a third-party api to retrieve the public ip or not, default to using own endpoint.
  - Muggle friendly network stability test tool, (testing ping, dns resolution, etc... a few simple metrics to see if everything is alright or not)
  - Speedtest? I can try but I don't know how yet (without using a pre-existing api), any ideas on this are always welcome.
- **QR Code generator**
  - Very simply encode whatever you input / upload into the qr code.
- **PDF Utilities**
  - PDF editor, upload 1 or more pdf files (will ask how to merge, before after or in between some pages)
    - Overview of all pages in a grid
      - (sidebar, right of the grid, only visible on selection).
      - (drag and drop support for re-arranging)
      - (select boxes for batch operations, can be done from the sidebar, all operation have text labels)
        - rotate clockwise
        - rotate counter-clockwise
        - flip horizontally
        - flip vertically
        - \-\-\-
        - insert something before (opens file open dialog)
        - insert something after (opens file open dialog)
        - \-\-\-
        - duplicate
        - remove
      - (clicking on a page opens it for large screen preview with a clear close button and key-hooks on `esc`)
        - Future version could see this turn into a full fletched PDF editor 
    - top bar, above grid shows uploaded pdf files, the name of the new document and buttons to save the new files
  - Quick Merge (specify in which order to merge the files)
  - Quick Rotate (rotate entire document or select)
  - Flatten & Trim PDF (trim page overflows. flatten all pdf layers into 1)
- **Developer Utilities**
  - Encode / Decode (eg. base64)
  - Convert (eg. json to xml, ...)
  - Epoch/Unix time calculation, formatters, readers, etc...
  - Test Servers
    - socket
    - html
    - coap
    - mqtt
  - Epoch/unix time operations (read, create, etc...)
  - Advanced network inspection, etc... tools.
