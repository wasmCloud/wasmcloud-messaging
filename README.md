# wasmCloud Messaging Interface (wit)
This repository contains the wit definition and any additional documentation necessary for the wasmCloud Messaging Interface (wit). This interface is used by actors to send and receive messages from a host runtime. A capability provider implementation is responsible for implementing this interface.

This interface is defined in [wit](./wit/messaging.wit). This is an interim solution to provide a wit-based messaging provider contract to wasmCloud components until such time as the [wasi-messaging](https://github.com/WebAssembly/wasi-messaging) specification stabilizes.

Wit-based wasmCloud interfaces are only available in the newest versions of wasmCloud hosts that utilize the [wasmCloud](https://github.com/wasmcloud/wasmcloud) crates.

The [wasmCloud Actor SDK](https://github.com/wasmCloud/wasmCloud/tree/main/crates/actor) will automatically provide the necessary translation/"fill" for components using this interface.