---
title: "Mono Types — First-Class Containers for Datalog"
collection: publications
permalink: /publication/2025-06-10-mono_types
excerpt: 'We propose mono types, a new abstraction for programming Datalog. Mono types behave like first-class containers that can be stored in relations and to which elements can be added decentrally. But, mono types are more than just containers: They provide a read operation that can yield any result as long as it monotonically grows with each added element and is independent of the order in which elements are added to the container. This design permits a wide range of mono types (e.g., sets, maps, and aggregations), yet guarantees mono types can be integrated into Datalog without jeopardizing Datalog’s least fixed-point semantics.'
date: 2025-06-10
venue: 'ECOOP'
paperurl: 'https://doi.org/10.4230/LIPIcs.ECOOP.2025.5'
citation: 'Runqing Xu, David Klopp, Sebastian Erdweg. (2025). &quot;Mono Types — First-Class Containers for Datalog.&quot; <i> ECOOP (2025) </i>.'
---
We propose mono types, a new abstraction for programming Datalog. Mono types behave like first-class containers that can be stored in relations and to which elements can be added decentrally. But, mono types are more than just containers: They provide a read operation that can yield any result as long as it monotonically grows with each added element and is independent of the order in which elements are added to the container. This design permits a wide range of mono types (e.g., sets, maps, and aggregations), yet guarantees mono types can be integrated into Datalog without jeopardizing Datalog’s least fixed-point semantics. We develop a theory for mono types, which includes constructions for complex mono types, equivalence relation for mono types, and properties about semantics-preserving mono-type transformations. This theory ensures sound Datalog integration and justifies crucial compiler optimizations for mono types. Together, these techniques demonstrate that mono types provide abstraction without regret: We demonstrate in two case studies that programs become easier to write with mono types, while their performance also improves drastically.

[Download paper here](https://www.pl.informatik.uni-mainz.de/files/2025/04/datalog-mono-types.pdf)
