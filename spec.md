# Introduction
This specification will introduce the UOR-DPL schemas first and then explain how they are leveraged. 

# Schemas
## UOR Element
The [UOR Element](./core/element.json) is a variable. It is able to represent data or a pointer to data along with logic encapsulated within that data. In the same way that many general programming languages store variables in memory, UOR-DPL leverages Open Containers Initiative (OCI) as its default storage mechanism.

The locatorType field of the UOR Element is used to specify the protocol and driver used to perform CRUD operations on the data expressed within the UOR Element resource field. The location field of the UOR Element is used to represent parameters that are passed to the driver specified in the locatorType field.

The resourceType field of the UOR Element is used to specify the type of data that is stored within the UOR Element resource field. The type definition referenced by the resourceType field includes the data structure and methods of the data in the UOR Element resource field. The resource field of the UOR Element is used to express the data represented by the UOR Element.

## Built-in Types

[Atomic Signature](./core/built-in/atomic_signature.json): An Atomic Signature is a type that represents a cryptographic signatureS.

[UOR Class](./class.md): A UOR Class is a type that represents a data structure and methods that can be used to manipulate that data structure.

[OCI Descriptor](./descriptor.md): An OCI Descriptor is a type that represents a pointer to data. 

[UOR Runtime](./runtime.md): A UOR Runtime is a type that represents a runtime module.

[UOR Statement](./statement.md): A UOR Statement is a type that represents linked data.

## Extensions

[git](./extensions/git.json): The git extension is used to represent a git repository, but can also be used to represent a unix file system.
