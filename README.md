# @zeeklog/react-vite-component-tagger

A Vite plugin that automatically adds data-dyad-id and data-dyad-name attributes to your React components. This public mirror is derived from the Apache-2.0 package originally published by Dyad.

## Installation

```bash
npm install @zeeklog/react-vite-component-tagger
# or
yarn add @zeeklog/react-vite-component-tagger
# or
pnpm add @zeeklog/react-vite-component-tagger
```

## Usage

Add the plugin to your vite.config.ts file:

```ts
import { defineConfig } from "vite";
import react from "@vitejs/plugin-react";
import zeeklogTagger from "@zeeklog/react-vite-component-tagger";

export default defineConfig({
  plugins: [react(), zeeklogTagger()],
});
```

The plugin automatically adds data-dyad-id and data-dyad-name to React components. The data-dyad-id value identifies each component instance as path/to/file.tsx:line:column.

## Source

This repository mirrors the published Dyad build. It retains the original Apache-2.0 license and attribution.
