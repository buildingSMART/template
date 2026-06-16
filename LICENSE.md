# Table of Contents

1. [Copyright Notice](#copyright-notice)
   1. [No Warranty Notice](#no-warranty-notice)
   2. [Trademark Notice](#trademark-notice)
   3. [Copyright Exclusion Notice](#copyright-exclusion-notice)
   4. [Correspondence Notice](#correspondence-notice)
2. [License](#license)
   1. [Final publications - the CC BY-ND 4.0](#the-cc-by-nd-40-for-releases)
   2. [The Apache License 2.0 for Work in Progress](#the-apache-license-20-for-work-in-progress)

Draft collaboration licence - the Apache License 2.0
Final publications - the CC BY-ND 4.0

# Copyright Notice

This repository contains a **development version** of the Industry Foundation Classes.
Official publications are available under an [open license](#license) on [https://standards.buildingsmart.org/IFC/RELEASE/](https://standards.buildingsmart.org/IFC/RELEASE/).

Copyright © 1996-2026 buildingSMART International Limited. All rights reserved.
Any technical documentation made available by buildingSMART International Limited is the copyrighted work of buildingSMART International Limited and is owned by buildingSMART International Limited. It may be photocopied, used in software development, or translated into another computer language without prior written consent from buildingSMART International Limited, provided that full attribution is given. Prior written consent is required if changes are made to the technical specification.

## No Warranty Notice
This material is delivered to you as is, and buildingSMART International Limited makes no warranty of any kind with regard to it, including, but not limited to, the implied warranties as to its accuracy or fitness for a particular purpose. Any use of the technical documentation or the information contained therein is at the user's own risk. Documentation may include technical or other inaccuracies or typographical errors. buildingSMART International Limited shall not be liable for errors contained therein or for incidental or consequential damages in connection with the furnishing, performance or use of the material. The information contained in this document is subject to change without notice.

## Trademark Notice
Industry Foundation Class™, IFC™, ifcXML™, and the logos  are trademarks of buildingSMART International Limited and should be given appropriate credits. Membership of any Chapter affiliated to buildingSMART International Limited, as indicated by the appellation buildingSMART Member, or use of a trademark in conjunction with any documentation developed using IFC documentation, does not imply responsibility for or approval of that documentation by buildingSMART International Limited.

## Copyright Exclusion Notice
Parts of the IFC documentation contain material based on other international standards. The status of this material is clearly indicated throughout the documentation and is excluded from the Copyright of buildingSMART International Limited.

## Correspondence Notice
Inquiries should be addressed to buildingSMART International Limited at contact@buildingsmart.org.

# License

## Final Publications License - the CC BY-ND 4.0

<img width="150" alt="CC BY-ND" src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f0/CC_BY-ND.svg/330px-CC_BY-ND.svg.png">

Formal releases (static and immutable) are published under the `Creative Commons Attribution-NoDerivatives 4.0 International` license. 

You are **free to share** — copy and redistribute the material in any medium or format for any purpose, even commercially, under the following terms:
- **You must give appropriate credit** and provide a link to the license. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
- If you remix, transform, or build upon the material, **you may not distribute the modified material**.

To view a full text of this license, visit: http://creativecommons.org/licenses/by-nd/4.0/.

[Creative Commons - Frequently Asked Questions](https://creativecommons.org/faq/)

## buildingSMART Draft Collaboration Licence

Draft Contribution Licence ...
for the normative draft materials, backed by a Contributor Agreement that either assigns accepted contributions to bSI or gives bSI a very broad perpetual, irrevocable, sublicensable licence that expressly covers publication, modification, translation, integration into future editions, and sublicensing into ISO-facing outputs. 

TODO
 

## Software - the Apache License 2.0

The software and tooling under the **Apache 2.0**, and license test files, examples, and sample datasets under CC BY 4.0 or CC0, unless a particular example is itself normative or intended to remain under central control. 

[Apache License, Version 2.0 | Apache Software Foundation](https://www.apache.org/licenses/LICENSE-2.0)

## 

| Folder                      | Typical contents                                                                                     | Draft outbound licence                                                                          | Final publication outbound licence                                                                                        | Inbound contribution rule                                                                       | Notes                                                                                                                                                                                                      |
| --------------------------- | ---------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `schema/`                   | Current normative schema - EXPRESS, XSD, OWL, JSON schema, UML/XMI if it defines the standard        | **buildingSMART Draft Collaboration Licence**                                                         | **CC BY-ND 4.0** when published as part of the official standard                                                          | **CLA or assignment-strength contribution terms required**                                      | Treat as normative. Draft licence should allow forks, edits, and PRs only for contribution/review. Final should not allow derivative republication.                                                        |
| `reference-schema/`   | Historical or legacy reference schema, frozen prior releases                                         | Same as its historical release licence, usually **CC BY-ND 4.0** | Not part of a final release.                                                                | **CLA only if changes are accepted**                                                 |                                                                                                |
| `docs/`                     | Normative specification text, concept templates, entity/property docs, diagrams, explanatory clauses | **Draft Collaboration Licence**                                                                       | **CC BY-ND 4.0** for official specification docs                                                                          | **CLA required**                                      | If some docs are purely tutorials or educational guides, consider splitting them into `guidance/` and licensing under **CC BY 4.0** instead.                                                               |
| `examples/`                 | IFC files, snippets, sample models, sample payloads, educational examples                            | **Draft Collaboration Licence** if official/canonical. Otherwise **CC BY 4.0** or **CC0**             | **CC BY 4.0** or **CC0** for reusable examples. **CC BY-ND 4.0** only if the example is part of the normative publication | **CLA for official examples; lighter contribution terms acceptable for non-normative examples** | Best split: `examples/official/` and `examples/community/`. Official examples may affect interpretation; community examples should be easy to reuse.                                                       |
| `tests/`                    | Conformance tests, validation fixtures, expected results, invalid/valid IFC files                    | **CC0** or **CC BY 4.0** for data/fixtures. **Apache-2.0** for executable tests                       | Same as draft, unless a test becomes normative                                                                            | **CLA or DCO + explicit test contribution terms**                                               | Prefer permissive reuse. Vendors and open-source implementers need to copy tests freely. If tests encode normative assertions, keep governance strict but licence reuse broadly.                           |
| `code/` - repo scripts      | Build scripts, generators, validators, publication scripts, CI scripts, utilities                    | **Apache-2.0**                                                                                        | **Apache-2.0**                                                                                                            | **Inbound under Apache-2.0 plus CLA**                                                    | Do not use CC licences for software. Creative Commons recommends against CC licences for software, partly because CC licences lack software-specific source-code and patent terms. ([Creative Commons][1]) |
| `benchmark-implementation/` | Reference implementation, benchmark implementation, demonstrator, prototype software                 | **Apache-2.0**                                                                                        | **Apache-2.0**                                                                                                            | **CLA strongly recommended; otherwise DCO + Apache-2.0 inbound**                                | Apache-2.0 is suitable because it grants copyright rights and an express patent licence from contributors. ([apache.org][2])                                                                               |

Unless a folder contains a more specific notice, draft normative standard materials are licensed under the buildingSMART Draft Collaboration Licence. Software is licensed under Apache-2.0. Non-normative examples and test data are licensed under CC BY 4.0 or CC0, as marked. Official published standards are licensed separately under CC BY-ND 4.0.

\* bS-DCL - buildingSMART Draft Collaboration Licence ...

\*\* CLA - 

TODO: buildingSMART Contributor Licence Agreement (CLA)


