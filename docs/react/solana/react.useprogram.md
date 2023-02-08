---
slug: /solana/react.useprogram
title: useProgram() function
hide_title: true
displayed_sidebar: react
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## useProgram() function

Get an SDK instance to interact with any program

## Example

```jsx
import { useProgram } from "@thirdweb-dev/react/solana";

export default function Component() {
  const { program } = useProgram("{{program_address}}").program;

  // Now you can use the program in the rest of the component

  // For example, we can make a transaction
  async function functionCall() {
    await program.call("mint", ...);
  }

  ...
}
```

**Signature:**

```typescript
export declare function useProgram<TProgramType extends ProgramType>(
  address: RequiredParam<string>,
  type?: TProgramType,
): UseQueryResult<
  Readonly<{
    "nft-collection": NFTCollection;
    "nft-drop": NFTDrop;
    token: Token;
  }>[TProgramType],
  unknown
> & {
  program: Readonly<{
    "nft-collection": NFTCollection;
    "nft-drop": NFTDrop;
    token: Token;
  }>[TProgramType];
};
```

## Parameters

| Parameter | Type                                                    | Description                                                                 |
| --------- | ------------------------------------------------------- | --------------------------------------------------------------------------- |
| address   | [RequiredParam](./react.requiredparam.md)&lt;string&gt; | the address of the program to get an interface for                          |
| type      | TProgramType                                            | <i>(Optional)</i> optionally, pass in the program type to get static typing |

**Returns:**

UseQueryResult&lt;Readonly&lt;{ "nft-collection": NFTCollection; "nft-drop": NFTDrop; token: Token; }&gt;\[TProgramType\], unknown&gt; &amp; { program: Readonly&lt;{ "nft-collection": NFTCollection; "nft-drop": NFTDrop; token: Token; }&gt;\[TProgramType\]; }