# bb-poc-fixtures

Static fixtures for **authorized** bug-bounty testing. Nothing here attacks anything by
itself: these are inert documents that a target application may be asked to fetch as part
of a proof of concept, so that the proof does not depend on an ephemeral tunnel.

`client-metadata.json` is an OAuth Client ID Metadata Document used to answer one
question: does an authorization server that advertises
`client_id_metadata_document_supported` actually fetch and accept such a document?
It declares a public client with no secret and a redirect URI on this same origin.

Reported through YesWeHack (handle: goofy). No credentials, no secrets, no target data.
