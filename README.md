# VScode-Extension-Development

"IT 종사자를 위한 스트레스 및 번아웃 관리 확장 프로그램(Extensions), 
메니저(mén_ager)"

IT 산업 종사자들 중 특히, 개발자들은 번아웃이 발생할 확률이 높고 스트레스를 관리하기 힘들다.
따라서 업무 중에서 자주 사용하는 도구들(GitHub, Chrome, Visual Studio, Adobe, etc.) 
확장 프로그램(Extension)을 제공해서 스트레스 관리 및 번아웃을 방지할 수 있게 도와주려고 한다.


![image](https://github.com/youngmin9/VScode-Extension-Development/assets/93260170/392c70ae-cc91-4456-83f5-5b86dad01752)

UI 구성 component score
본인의 상태(번아웃 점수)
일일 업무 목표(달성 점수)

기존 설문조사 링크
https://i6zvqipg2sh.typeform.com/to/A6K33zQG

<h1 align="center">
VS Code Extension Samples
</h1>

This repository contains sample code illustrating the VS Code extension API. Each sample is a self-contained extension that explains one topic in [VS Code API](https://code.visualstudio.com/api/references/vscode-api) or VS Code's [Contribution Points](https://code.visualstudio.com/api/references/contribution-points). You can read, play with or adapt from these samples to create your own extensions.

You can expect from each sample:
- An explanation of its functionality
- A gif or screenshot demonstrating its usage
- Link to a guide on VS Code website, if it has one
- Listing of used VS Code API and Contribution Points
- Code of the same style, enforced using ESLint

## Prerequisites

You need to have [node](https://nodejs.org/en/) and [npm](https://nodejs.org/en/) installed on your system to run the examples. It is recommended to use the node version used for VS Code development itself which is documented [here](https://github.com/Microsoft/vscode/wiki/How-to-Contribute#prerequisites)

## Usage

- `git clone https://github.com/Microsoft/vscode-extension-samples`
- `code <any-sample-folder>`
- `npm install` in the terminal, then `F5` to run the sample
- Alternatively, follow the instructions in each sample's README for setting up and running the sample

## Getting Started

- [Hello World Sample](helloworld-sample): The Hello World sample for VS Code. See [Extension Anatomy](https://code.visualstudio.com/api/get-started/extension-anatomy) documentation.
- [Hello World Minimal Sample](helloworld-minimal-sample): A minimal version of Hello World Sample written in JavaScript.
- [Hello World Test Sample](helloworld-test-sample): Hello World sample with extension integration test. See [Testing Extensions](https://code.visualstudio.com/api/working-with-extensions/testing-extension) documentation.
- [Hello World Web Sample](helloworld-web-sample): The Hello World sample for VS Code Web. See the [Web Extensions](https://code.visualstudio.com/api/extension-guides/web-extensions) guide.

## Samples

<!-- SAMPLES_BEGIN -->
| Sample | Guide on VS Code Website | API & Contribution |
| ------ | ----- | --- |
| [Webview Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/webview-sample) | [/api/extension-guides/webview](https://code.visualstudio.com/api/extension-guides/webview) | [window.createWebviewPanel](https://code.visualstudio.com/api/references/vscode-api#window.createWebviewPanel)<br>[window.registerWebviewPanelSerializer](https://code.visualstudio.com/api/references/vscode-api#window.registerWebviewPanelSerializer) |
| [Webview View Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/webview-view-sample) | N/A | [window.registerWebviewViewProvider](https://code.visualstudio.com/api/references/vscode-api#window.registerWebviewViewProvider) |
| [Webview Codicons Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/webview-codicons-sample) | N/A |  |
| [Status Bar Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/statusbar-sample) | N/A | [window.createStatusBarItem](https://code.visualstudio.com/api/references/vscode-api#window.createStatusBarItem)<br>[StatusBarItem](https://code.visualstudio.com/api/references/vscode-api#StatusBarItem) |
| [Tree View Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/tree-view-sample) | [/api/extension-guides/tree-view](https://code.visualstudio.com/api/extension-guides/tree-view) | [window.createTreeView](https://code.visualstudio.com/api/references/vscode-api#window.createTreeView)<br>[window.registerTreeDataProvider](https://code.visualstudio.com/api/references/vscode-api#window.registerTreeDataProvider)<br>[TreeView](https://code.visualstudio.com/api/references/vscode-api#TreeView)<br>[TreeDataProvider](https://code.visualstudio.com/api/references/vscode-api#TreeDataProvider)<br>[contributes.views](https://code.visualstudio.com/api/references/contribution-points#contributes.views)<br>[contributes.viewsContainers](https://code.visualstudio.com/api/references/contribution-points#contributes.viewsContainers) |
| [Task Provider Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/task-provider-sample) | [/api/extension-guides/task-provider](https://code.visualstudio.com/api/extension-guides/task-provider) | [tasks.registerTaskProvider](https://code.visualstudio.com/api/references/vscode-api#tasks.registerTaskProvider)<br>[Task](https://code.visualstudio.com/api/references/vscode-api#Task)<br>[ShellExecution](https://code.visualstudio.com/api/references/vscode-api#ShellExecution)<br>[contributes.taskDefinitions](https://code.visualstudio.com/api/references/contribution-points#contributes.taskDefinitions) |
| [Multi Root Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/basic-multi-root-sample) | N/A | [workspace.getWorkspaceFolder](https://code.visualstudio.com/api/references/vscode-api#workspace.getWorkspaceFolder)<br>[workspace.onDidChangeWorkspaceFolders](https://code.visualstudio.com/api/references/vscode-api#workspace.onDidChangeWorkspaceFolders) |
| [Completion Provider Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/completions-sample) | N/A | [languages.registerCompletionItemProvider](https://code.visualstudio.com/api/references/vscode-api#languages.registerCompletionItemProvider)<br>[CompletionItem](https://code.visualstudio.com/api/references/vscode-api#CompletionItem)<br>[SnippetString](https://code.visualstudio.com/api/references/vscode-api#SnippetString) |
| [Code Actions Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/code-actions-sample) | N/A | [languages.registerCodeActionsProvider](https://code.visualstudio.com/api/references/vscode-api#languages.registerCodeActionsProvider)<br>[CodeActionProvider](https://code.visualstudio.com/api/references/vscode-api#CodeActionProvider) |
| [File System Provider Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/fsprovider-sample) | N/A | [workspace.registerFileSystemProvider](https://code.visualstudio.com/api/references/vscode-api#workspace.registerFileSystemProvider) |
| [Editor Decorator Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/decorator-sample) | N/A | [TextEditor.setDecorations](https://code.visualstudio.com/api/references/vscode-api#TextEditor.setDecorations)<br>[DecorationOptions](https://code.visualstudio.com/api/references/vscode-api#DecorationOptions)<br>[DecorationInstanceRenderOptions](https://code.visualstudio.com/api/references/vscode-api#DecorationInstanceRenderOptions)<br>[ThemableDecorationInstanceRenderOptions](https://code.visualstudio.com/api/references/vscode-api#ThemableDecorationInstanceRenderOptions)<br>[window.createTextEditorDecorationType](https://code.visualstudio.com/api/references/vscode-api#window.createTextEditorDecorationType)<br>[TextEditorDecorationType](https://code.visualstudio.com/api/references/vscode-api#TextEditorDecorationType)<br>[contributes.colors](https://code.visualstudio.com/api/references/contribution-points#contributes.colors) |
| [L10n Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/l10n-sample) | N/A |  |
| [Terminal Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/terminal-sample) | N/A | [window.createTerminal](https://code.visualstudio.com/api/references/vscode-api#window.createTerminal)<br>[window.onDidChangeActiveTerminal](https://code.visualstudio.com/api/references/vscode-api#window.onDidChangeActiveTerminal)<br>[window.onDidCloseTerminal](https://code.visualstudio.com/api/references/vscode-api#window.onDidCloseTerminal)<br>[window.onDidOpenTerminal](https://code.visualstudio.com/api/references/vscode-api#window.onDidOpenTerminal)<br>[window.Terminal](https://code.visualstudio.com/api/references/vscode-api#window.Terminal)<br>[window.terminals](https://code.visualstudio.com/api/references/vscode-api#window.terminals) |
| [Extension Terminal Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/extension-terminal-sample) | N/A | [window.createTerminal](https://code.visualstudio.com/api/references/vscode-api#window.createTerminal)<br>[window.Pseudoterminal](https://code.visualstudio.com/api/references/vscode-api#window.Pseudoterminal)<br>[window.ExtensionTerminalOptions](https://code.visualstudio.com/api/references/vscode-api#window.ExtensionTerminalOptions) |
| [Color Theme Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/theme-sample) | [/api/extension-guides/color-theme](https://code.visualstudio.com/api/extension-guides/color-theme) | [contributes.themes](https://code.visualstudio.com/api/references/contribution-points#contributes.themes) |
| [Product Icon Theme Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/product-icon-theme-sample) | [/api/extension-guides/product-icon-theme](https://code.visualstudio.com/api/extension-guides/product-icon-theme) | [contributes.productIconThemes](https://code.visualstudio.com/api/references/contribution-points#contributes.productIconThemes) |
| [Vim Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/vim-sample) | N/A | [commands](https://code.visualstudio.com/api/references/vscode-api#commands)<br>[StatusBarItem](https://code.visualstudio.com/api/references/vscode-api#StatusBarItem)<br>[window.createStatusBarItem](https://code.visualstudio.com/api/references/vscode-api#window.createStatusBarItem)<br>[TextEditorCursorStyle](https://code.visualstudio.com/api/references/vscode-api#TextEditorCursorStyle)<br>[window.activeTextEditor](https://code.visualstudio.com/api/references/vscode-api#window.activeTextEditor)<br>[Position](https://code.visualstudio.com/api/references/vscode-api#Position)<br>[Range](https://code.visualstudio.com/api/references/vscode-api#Range)<br>[Selection](https://code.visualstudio.com/api/references/vscode-api#Selection)<br>[TextEditor](https://code.visualstudio.com/api/references/vscode-api#TextEditor)<br>[TextEditorRevealType](https://code.visualstudio.com/api/references/vscode-api#TextEditorRevealType)<br>[TextDocument](https://code.visualstudio.com/api/references/vscode-api#TextDocument) |
| [webpack-sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/webpack-sample) | N/A |  |
| [Source Control Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/source-control-sample) | [/api/extension-guides/scm-provider](https://code.visualstudio.com/api/extension-guides/scm-provider) | [workspace.workspaceFolders](https://code.visualstudio.com/api/references/vscode-api#workspace.workspaceFolders)<br>[SourceControl](https://code.visualstudio.com/api/references/vscode-api#SourceControl)<br>[SourceControlResourceGroup](https://code.visualstudio.com/api/references/vscode-api#SourceControlResourceGroup)<br>[scm.createSourceControl](https://code.visualstudio.com/api/references/vscode-api#scm.createSourceControl)<br>[TextDocumentContentProvider](https://code.visualstudio.com/api/references/vscode-api#TextDocumentContentProvider)<br>[contributes.menus](https://code.visualstudio.com/api/references/contribution-points#contributes.menus) |
| [Commenting API Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/comment-sample) | N/A |  |
| [Document Editing Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/document-editing-sample) | N/A | [commands](https://code.visualstudio.com/api/references/vscode-api#commands) |
| [Custom Data Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/custom-data-sample) | [/api/extension-guides/custom-data-extension](https://code.visualstudio.com/api/extension-guides/custom-data-extension) |  |
| [CodeLens Provider Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/codelens-sample) | N/A | [languages.registerCodeLensProvider](https://code.visualstudio.com/api/references/vscode-api#languages.registerCodeLensProvider)<br>[CodeLensProvider](https://code.visualstudio.com/api/references/vscode-api#CodeLensProvider)<br>[CodeLens](https://code.visualstudio.com/api/references/vscode-api#CodeLens) |
| [Call Hierarchy Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/call-hierarchy-sample) | N/A | [languages.registerCallHierarchyProvider](https://code.visualstudio.com/api/references/vscode-api#languages.registerCallHierarchyProvider)<br>[CallHierarchyProvider](https://code.visualstudio.com/api/references/vscode-api#CallHierarchyProvider)<br>[CallHierarchyItem](https://code.visualstudio.com/api/references/vscode-api#CallHierarchyItem)<br>[CallHierarchyOutgoingCall](https://code.visualstudio.com/api/references/vscode-api#CallHierarchyOutgoingCall)<br>[CallHierarchyIncomingCall](https://code.visualstudio.com/api/references/vscode-api#CallHierarchyIncomingCall) |
| [Custom Editors Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/custom-editor-sample) | [/api/extension-guides/custom-editors](https://code.visualstudio.com/api/extension-guides/custom-editors) | [window.registerCustomEditorProvider](https://code.visualstudio.com/api/references/vscode-api#window.registerCustomEditorProvider)<br>[CustomTextEditorProvider](https://code.visualstudio.com/api/references/vscode-api#CustomTextEditorProvider)<br>[contributes.customEditors](https://code.visualstudio.com/api/references/contribution-points#contributes.customEditors) |
| [Semantic tokens](https://github.com/Microsoft/vscode-extension-samples/tree/main/semantic-tokens-sample) | [/api/language-extensions/semantic-highlight-guide](https://code.visualstudio.com/api/language-extensions/semantic-highlight-guide) | [languages.registerDocumentSemanticTokensProvider](https://code.visualstudio.com/api/references/vscode-api#languages.registerDocumentSemanticTokensProvider)<br>[vscode.DocumentSemanticTokensProvider](https://code.visualstudio.com/api/references/vscode-api#vscode.DocumentSemanticTokensProvider) |
| [Test Provider Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/test-provider-sample) | N/A |  |
| [Getting Started Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/getting-started-sample) | N/A |  |
| [notebook-renderer-sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/notebook-renderer-sample) | [/api/extension-guides/notebook#notebook-renderer](https://code.visualstudio.com/api/extension-guides/notebook#notebook-renderer) | [contributes.notebookRenderer](https://code.visualstudio.com/api/references/contribution-points#contributes.notebookRenderer) |
| [notebook-extend-markdown-renderer-sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/notebook-extend-markdown-renderer-sample) | [/api/extension-guides/notebook#notebook-renderer](https://code.visualstudio.com/api/extension-guides/notebook#notebook-renderer) | [contributes.notebookRenderer](https://code.visualstudio.com/api/references/contribution-points#contributes.notebookRenderer) |
<!-- SAMPLES_END -->

### Language Server Protocol Samples

<!-- LSP_SAMPLES_BEGIN -->
| Sample | Guide on VS Code Website | API & Contribution |
| ------ | ----- | --- |
| [Snippet Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/snippet-sample) | [/api/language-extensions/snippet-guide](https://code.visualstudio.com/api/language-extensions/snippet-guide) | [contributes.snippets](https://code.visualstudio.com/api/references/contribution-points#contributes.snippets) |
| [Language Configuration Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/language-configuration-sample) | [/api/language-extensions/language-configuration-guide](https://code.visualstudio.com/api/language-extensions/language-configuration-guide) | [contributes.languages](https://code.visualstudio.com/api/references/contribution-points#contributes.languages) |
| [LSP Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/lsp-sample) | [/api/language-extensions/language-server-extension-guide](https://code.visualstudio.com/api/language-extensions/language-server-extension-guide) |  |
| [LSP Log Streaming Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/lsp-log-streaming-sample) | N/A |  |
| [LSP Multi Root Server Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/lsp-multi-server-sample) | https://github.com/Microsoft/vscode/wiki/Extension-Authoring:-Adopting-Multi-Root-Workspace-APIs#language-client--language-server |  |
| [LSP Web Extension Sample](https://github.com/Microsoft/vscode-extension-samples/tree/main/lsp-web-extension-sample) | [/api/language-extensions/language-server-extension-guide](https://code.visualstudio.com/api/language-extensions/language-server-extension-guide) |  |
<!-- LSP_SAMPLES_END -->

## License

Copyright (c) Microsoft Corporation. All rights reserved.

Licensed under the [MIT](https://github.com/microsoft/vscode-extension-samples/blob/main/LICENSE) License.


소비자에게 효용을 제시 및 제공하기 위해선 정량적인 지표가 있어야 하고, 그것이 stress management score로 환산하기 편한 '시간'이라고 우선 접근했으며, 그 중 '시간 단위당 개발자가 짠 코드 줄(line) 수'로 관리하기 비교하거나 체력바 형태(gamification)로 제공하면 어떨까. 라는 발상의 검증 과정이 2월까지 선행되어야 하며, 기본 튜토리얼의 steps 및 sample 확인중

---
