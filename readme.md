# Demo for Triptych Architecture in a single-module maven project

This project is intended to demonstrate the Triptych naming conventions compared to the Hexagonal / Ports and Adapters Naming conventions.
It is not intended as a template project for new projects.
Other projects exist for that purpose (recommended: https://github.com/svene/2026-07-26_quarkus-hexagon-demo-mm-per-tech)

- Primary Adapter: * -> *Receiver
- Core/Primary Port: *Port -> *API
- Core: *Handler -> *Handler (unchanged)
- Core/Secondary Port: *Port -> *SPI
- Secondary Adapter: *Service -> *Service (unchanged)

## Usage

http://localhost:8080/hello

## Misc
created using sdkman command `quarkus`:

`quarkus create app --name=quarkus-triptych-architecturedemo-sm --maven --java=21 --wrapper --code org.svenehrke.demo:quarkus-triptych-architecture-demo-sm:1.0`

## Further Info

- https://herbertograca.com/2017/11/16/explicit-architecture-01-ddd-hexagonal-onion-clean-cqrs-how-i-put-it-all-together/
- 
