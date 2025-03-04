---
id: node-git-server.httpduplex
hide_title: true
custom_edit_url: null
title: HttpDuplex class
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) > [node-git-server](./node-git-server.md) > [HttpDuplex](./node-git-server.httpduplex.md)

## HttpDuplex class

<b>Signature:</b>

```typescript
export declare class HttpDuplex extends EventEmitter
```

**Extends:** EventEmitter

## Constructors

| Constructor                                                                   | Modifiers | Description                                                                                                                                                      |
| ----------------------------------------------------------------------------- | --------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [(constructor)(input, output)](./node-git-server.httpduplex._constructor_.md) |           | Constructs a proxy object over input and output resulting in a unified stream. Generally meant to combine request and response streams in the http.request event |

## Properties

| Property                                                             | Modifiers | Type                     | Description                                                                                                                                                                                                                                                  |
| -------------------------------------------------------------------- | --------- | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------- |
| [complete](./node-git-server.httpduplex.complete.md)                 |           | boolean                  |                                                                                                                                                                                                                                                              |
| [connection](./node-git-server.httpduplex.connection.md)             |           | import("net").Socket     | Reference to the underlying socket for the request connection.                                                                                                                                                                                               |
| [cwd](./node-git-server.httpduplex.cwd.md)                           |           | string                   | undefined                                                                                                                                                                                                                                                    |                                         |
| [exists](./node-git-server.httpduplex.exists.md)                     |           | boolean                  | undefined                                                                                                                                                                                                                                                    |                                         |
| [headers](./node-git-server.httpduplex.headers.md)                   |           | http.IncomingHttpHeaders | Request/response headers. Key-value pairs of header names and values. Header names are always lower-case.                                                                                                                                                    |
| [httpVersion](./node-git-server.httpduplex.httpversion.md)           |           | string                   | Requested HTTP Version sent by the client. Usually either '1.0' or '1.1'                                                                                                                                                                                     |
| [httpVersionMajor](./node-git-server.httpduplex.httpversionmajor.md) |           | number                   | First integer in the httpVersion string                                                                                                                                                                                                                      |
| [httpVersionMinor](./node-git-server.httpduplex.httpversionminor.md) |           | number                   | Second integer ni the httpVersion string                                                                                                                                                                                                                     |
| [method](./node-git-server.httpduplex.method.md)                     |           | string                   | undefined                                                                                                                                                                                                                                                    | Request method of the incoming request. |
| [readable](./node-git-server.httpduplex.readable.md)                 |           | boolean                  | Is this stream readable.                                                                                                                                                                                                                                     |
| [repo](./node-git-server.httpduplex.repo.md)                         |           | string                   | undefined                                                                                                                                                                                                                                                    |                                         |
| [req](./node-git-server.httpduplex.req.md)                           |           | http.IncomingMessage     | A IncomingMessage created by http.Server or http.ClientRequest usually passed as the first parameter to the 'request' and 'response' events. Implements Readable Stream interface but may not be a decendant thereof.                                        |
| [res](./node-git-server.httpduplex.res.md)                           |           | http.ServerResponse      | Created http.server. Passed as the second parameter to the 'request' event. The response implements Writable Stream interface but isn't a descendent thereof.                                                                                                |
| [socket](./node-git-server.httpduplex.socket.md)                     |           | import("net").Socket     | net.Socket object associated with the connection.                                                                                                                                                                                                            |
| [statusCode](./node-git-server.httpduplex.statuscode.md)             |           | number                   | The HTTP status code. Generally assigned before sending headers for a response to a client.                                                                                                                                                                  |
| [statusMessage](./node-git-server.httpduplex.statusmessage.md)       |           | string                   | Controls the status message sent to the client as long as an explicit call to response.writeHead() isn't made If ignored or the value is undefined, the default message corresponding to the status code will be used.                                       |
| [trailers](./node-git-server.httpduplex.trailers.md)                 |           | NodeJS.Dict\<string\>    | Request/response trailer headers. Just like except these are only written after the initial response to the client. This object is only populated at the 'end' event and only work if a 'transfer-encoding: chunked' header is sent in the initial response. |
| [url](./node-git-server.httpduplex.url.md)                           |           | string                   | undefined                                                                                                                                                                                                                                                    | Request URL string.                     |
| [writable](./node-git-server.httpduplex.writable.md)                 |           | boolean                  |                                                                                                                                                                                                                                                              |

## Methods

| Method                                                                                     | Modifiers | Description                                                                                                    |
| ------------------------------------------------------------------------------------------ | --------- | -------------------------------------------------------------------------------------------------------------- |
| [accept()](./node-git-server.httpduplex.accept.md)                                         |           |                                                                                                                |
| [cork()](./node-git-server.httpduplex.cork.md)                                             |           | Buffers written data in memory. This data will be flushed when either the uncork or end methods are called.    |
| [destroy()](./node-git-server.httpduplex.destroy.md)                                       |           |                                                                                                                |
| [end(reason)](./node-git-server.httpduplex.end.md)                                         |           |                                                                                                                |
| [reject(code, msg)](./node-git-server.httpduplex.reject.md)                                |           |                                                                                                                |
| [setHeader(arg0, arg1)](./node-git-server.httpduplex.setheader.md)                         |           |                                                                                                                |
| [uncork()](./node-git-server.httpduplex.uncork.md)                                         |           | Flushes all data buffered since cork() was called.                                                             |
| [writeHead(statusCode, statusMessage, headers)](./node-git-server.httpduplex.writehead.md) |           | Sends a response header to the client request. Must only be called one time and before calling response.end(). |
