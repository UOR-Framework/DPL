This is the [Descriptor](./core/built-in/oci_descriptor.json) Specification of the Universal Object Reference (UOR) Declarative Programming Language (DPL).

The Descriptor Specification describes how a pointer in UOR-DPL is expressed.

The built-in UOR-DPL pointer type is an OCI Descriptor. The OCI Descriptor is used to describe the storage location of UOR formatted data. The OCI Descriptor is defined by the OCI Image Specification.

The only prescribed formatting of the OCI Descriptor for the UOR DPL use-case is that the URLs field in the OCI Descriptor MUST convey the URI to the OCI namespace that contains the OCI artifact referenced by the OCI Descriptor. 