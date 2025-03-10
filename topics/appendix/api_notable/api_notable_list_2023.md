# Notable Changes in IntelliJ Platform and Plugins API 2023.*

<!-- Copyright 2000-2023 JetBrains s.r.o. and other contributors. Use of this source code is governed by the Apache 2.0 license that can be found in the LICENSE file. -->

<link-summary>List of known Notable API Changes in 2023.*</link-summary>

_Early Access Program_ (EAP) releases of upcoming versions are available [here](https://eap.jetbrains.com).


<include from="tools_gradle_intellij_plugin.md" element-id="gradle_plugin_223_problem"/>

## 2023.2

### IntelliJ Platform 2023.2

## 2023.1

### IntelliJ Platform 2023.1

Nested Index Access
: Accessing index data in [nested calls](file_based_indexes.md#nested-index-access) is now possible.

File Type Index Topic
: [`FileTypeIndex.IndexChangeListener`](%gh-ic-master%/platform/indexing-api/src/com/intellij/psi/search/FileTypeIndex.java) allows monitoring addition/removal of files by `FileType`.

Run Annotator During Indexing
: [Annotators](syntax_highlighting_and_error_highlighting.md#annotator) can implement `DumbAware` to run during indexing (e.g., providing additional syntax highlighting).

Obsolete API
: Newly introduced `ApiStatus.@Obsolete` marks API that should not be used for new code, see [](verifying_plugin_compatibility.md#obsolete-api).
