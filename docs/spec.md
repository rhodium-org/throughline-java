# Google Java style — throughline source

This document is **generated from the graph** by `tl docs`; `tl docs --check` gates it in CI. The prose headings are hand-owned — everything between `tl:*` markers is injected from the YAML items, so the published spec can never drift from the graph.

This source re-expresses the **Google Java Style Guide** as a grounded IDD graph: each major section is a `user_requirement`, and every individual rule is a `system_requirement` that `implements` its section. The guide reference lives in `attrs.source_ref`; the throughline UIDs are this source's own and immutable — a consumer cites a rule as `java:SR-0001`, never by section name.

It carries
<!-- tl:count type == 'user_requirement' -->
8
<!-- tl:end --> sections and
<!-- tl:count type == 'system_requirement' -->
54
<!-- tl:end --> style rules.

## Purpose

<!-- tl:item INT-0001 -->
**INT-0001 — Java is written in one consistent, readable, maintainable style** — `intent`, status `proposed`

> The Google Java Style Guide exists so that Java across a large codebase reads as though written by one author: consistent source structure, formatting, naming and programming practices, so that any engineer can read and change code they did not write, and so that mechanical style questions are settled once rather than argued in every review.

**source_ref**: Google Java Style Guide
<!-- tl:end -->

## Source File Basics

<!-- tl:item UR-0001 -->
**UR-0001 — Source File Basics** — `user_requirement`, status `proposed`

> Rules governing a source file's name, encoding, whitespace and escape sequences.

*Derives from:* INT-0001

**source_ref**: Google Java Style Guide: Source File Basics
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google Java Style Guide: Source File Basics') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0001 | system_requirement | proposed | Name the file after its top-level class |
| SR-0002 | system_requirement | proposed | Encode source files in UTF-8 |
| SR-0003 | system_requirement | proposed | Use only the ASCII space and never tabs for whitespace |
| SR-0004 | system_requirement | proposed | Use special escape sequences over numeric escapes |
| SR-0005 | system_requirement | proposed | Choose actual character or Unicode escape for readability |
<!-- tl:end -->

## Source File Structure

<!-- tl:item UR-0002 -->
**UR-0002 — Source File Structure** — `user_requirement`, status `proposed`

> Rules governing the order of a file's contents, its package and import statements and its top-level class.

*Derives from:* INT-0001

**source_ref**: Google Java Style Guide: Source File Structure
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google Java Style Guide: Source File Structure') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0006 | system_requirement | proposed | Put license or copyright information first |
| SR-0007 | system_requirement | proposed | Give every file a non-wrapped package declaration |
| SR-0008 | system_requirement | proposed | Never use wildcard imports |
| SR-0009 | system_requirement | proposed | Do not line-wrap import statements |
| SR-0010 | system_requirement | proposed | Order imports as static then non-static, ASCII-sorted |
| SR-0011 | system_requirement | proposed | Import static nested classes with normal imports |
| SR-0012 | system_requirement | proposed | Keep exactly one top-level class per file |
| SR-0013 | system_requirement | proposed | Order class contents by a logical, explicable order |
| SR-0014 | system_requirement | proposed | Keep overloaded methods in one contiguous group |
<!-- tl:end -->

## Formatting — Braces and Blocks

<!-- tl:item UR-0003 -->
**UR-0003 — Formatting — Braces and Blocks** — `user_requirement`, status `proposed`

> Rules governing braces, block indentation, statements per line and the column limit.

*Derives from:* INT-0001

**source_ref**: Google Java Style Guide: Formatting — Braces and Blocks
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google Java Style Guide: Formatting — Braces and Blocks') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0015 | system_requirement | proposed | Always brace if, else, for, do and while |
| SR-0016 | system_requirement | proposed | Format nonempty blocks in K&R style |
| SR-0017 | system_requirement | proposed | Only close an empty block concisely when it stands alone |
| SR-0018 | system_requirement | proposed | Indent each new block by two spaces |
| SR-0019 | system_requirement | proposed | Follow each statement with a line break |
| SR-0020 | system_requirement | proposed | Keep lines within the 100-character column limit |
<!-- tl:end -->

## Formatting — Whitespace and Wrapping

<!-- tl:item UR-0004 -->
**UR-0004 — Formatting — Whitespace and Wrapping** — `user_requirement`, status `proposed`

> Rules governing line-wrapping, vertical and horizontal whitespace, alignment and grouping parentheses.

*Derives from:* INT-0001

**source_ref**: Google Java Style Guide: Formatting — Whitespace and Wrapping
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google Java Style Guide: Formatting — Whitespace and Wrapping') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0021 | system_requirement | proposed | Break lines at the highest syntactic level |
| SR-0022 | system_requirement | proposed | Indent continuation lines at least four spaces |
| SR-0023 | system_requirement | proposed | Separate class members with a single blank line |
| SR-0024 | system_requirement | proposed | Use single ASCII spaces for horizontal separation |
| SR-0025 | system_requirement | proposed | Do not require horizontal alignment |
| SR-0026 | system_requirement | proposed | Add grouping parentheses unless there is no ambiguity |
<!-- tl:end -->

## Formatting — Specific Constructs

<!-- tl:item UR-0005 -->
**UR-0005 — Formatting — Specific Constructs** — `user_requirement`, status `proposed`

> Rules governing enums, variable and array declarations, switch statements, annotations, comments, modifiers and literals.

*Derives from:* INT-0001

**source_ref**: Google Java Style Guide: Formatting — Specific Constructs
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google Java Style Guide: Formatting — Specific Constructs') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0027 | system_requirement | proposed | Format an enum class like other classes |
| SR-0028 | system_requirement | proposed | Declare only one variable per declaration |
| SR-0029 | system_requirement | proposed | Put array brackets on the type, not the variable |
| SR-0030 | system_requirement | proposed | Terminate or comment every switch statement group |
| SR-0031 | system_requirement | proposed | Place each type-level annotation on its own line |
| SR-0032 | system_requirement | proposed | Indent block comments with the surrounding code |
| SR-0033 | system_requirement | proposed | Order modifiers as recommended by the language specification |
| SR-0034 | system_requirement | proposed | Suffix long literals with an uppercase L |
<!-- tl:end -->

## Naming

<!-- tl:item UR-0006 -->
**UR-0006 — Naming** — `user_requirement`, status `proposed`

> Rules governing the characters, casing and choice of identifiers by kind.

*Derives from:* INT-0001

**source_ref**: Google Java Style Guide: Naming
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google Java Style Guide: Naming') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0035 | system_requirement | proposed | Use only ASCII letters, digits and permitted underscores in identifiers |
| SR-0036 | system_requirement | proposed | Do not use special prefixes or suffixes on identifiers |
| SR-0037 | system_requirement | proposed | Name packages in lowercase with no underscores |
| SR-0038 | system_requirement | proposed | Name classes in UpperCamelCase as nouns |
| SR-0039 | system_requirement | proposed | Name methods in lowerCamelCase as verbs |
| SR-0040 | system_requirement | proposed | Name constants in UPPER_SNAKE_CASE |
| SR-0041 | system_requirement | proposed | Name non-constant fields in lowerCamelCase |
| SR-0042 | system_requirement | proposed | Name parameters in lowerCamelCase and avoid one-character public names |
| SR-0043 | system_requirement | proposed | Name local variables in lowerCamelCase, never as constants |
| SR-0044 | system_requirement | proposed | Name type variables in one of the two accepted styles |
| SR-0045 | system_requirement | proposed | Derive camel case by the defined algorithm |
<!-- tl:end -->

## Programming Practices

<!-- tl:item UR-0007 -->
**UR-0007 — Programming Practices** — `user_requirement`, status `proposed`

> Rules governing @Override, caught exceptions, static-member access and finalizers.

*Derives from:* INT-0001

**source_ref**: Google Java Style Guide: Programming Practices
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google Java Style Guide: Programming Practices') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0046 | system_requirement | proposed | Mark every legal override with @Override |
| SR-0047 | system_requirement | proposed | Never silently ignore a caught exception |
| SR-0048 | system_requirement | proposed | Qualify a static member through its class |
| SR-0049 | system_requirement | proposed | Do not override or use finalizers |
<!-- tl:end -->

## Javadoc

<!-- tl:item UR-0008 -->
**UR-0008 — Javadoc** — `user_requirement`, status `proposed`

> Rules governing the formatting, summary and placement of Javadoc.

*Derives from:* INT-0001

**source_ref**: Google Java Style Guide: Javadoc
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google Java Style Guide: Javadoc') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0050 | system_requirement | proposed | Use the correct Javadoc block form |
| SR-0051 | system_requirement | proposed | Separate Javadoc paragraphs with a p tag |
| SR-0052 | system_requirement | proposed | Order Javadoc block tags and never leave them empty |
| SR-0053 | system_requirement | proposed | Open Javadoc with a summary fragment |
| SR-0054 | system_requirement | proposed | Document every visible class and member with the stated exceptions |
<!-- tl:end -->

