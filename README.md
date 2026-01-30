# d30.djs

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)](https://example.com/build)
[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://example.com/releases)
[![Discord](https://img.shields.io/discord/1234567890?color=7289da&label=Discord&logo=discord&logoColor=white)](https://discord.gg/d30djs)
[![Twitter](https://img.shields.io/twitter/follow/d30djs?style=social)](https://twitter.com/d30djs)

**d30.djs** is a versatile, resilient JavaScript-like runtime and scripting language developed by **AVIYON** as part of the **Unyversal Liquidity Exchange (ULE)** ecosystem. Inspired by D30 Impact Liquid---a non-Newtonian fluid that flows like water under normal conditions but hardens instantly upon impact---d30.djs embodies fluidity in development while providing stoic robustness under high-load or challenging scenarios. It serves as a universal frontend and backend solution, akin to Node.js, but optimized for seamless integration with blockchain environments, decentralized applications (dApps), and the ULE Stack.

d30.djs files use the `.djs` extension and can embed components from UNYSL (for statically typed logic), lofi.css (for programmable styling), and other ULE tools. It's designed for building everything from lightweight web apps to complex serverless backends, with built-in support for asynchronous operations, state management, and multichain interactions. Whether you're prototyping a quick script or scaling a production dApp, d30.djs "flows smoothly in its functionality while providing robust performance when faced with challenges."

## Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [The ULE Stack Integration](#the-ule-stack-integration)
- [d30.djs vs. Other Runtimes](#d30djs-vs-other-runtimes)
- [Why d30.djs?](#why-d30djs)
- [Installation](#installation)
- [Getting Started](#getting-started)
- [Examples](#examples)
- [Advanced Usage](#advanced-usage)
- [Performance and Resilience](#performance-and-resilience)
- [Development Workflow](#development-workflow)
- [The ULE Ecosystem](#the-ule-ecosystem)
- [Contributing](#contributing)
- [License](#license)

## Overview

d30.djs is more than just a JavaScript runtime---it's a bridge between traditional web development and the decentralized world of ULE. It handles both client-side rendering (e.g., in browsers) and server-side execution (e.g., on Aviyon Cloud nodes), making it ideal for full-stack dApps. Key philosophies:

- **Fluidity**: Write code that feels like modern JavaScript, with enhancements for async patterns, modules, and embeddings.
- **Hardening**: Built-in error recovery, load balancing, and impact resistance for high-traffic or fault-prone environments.
- **Universality**: Runs on any platform supported by the ULE Stack (Linux, Windows, Mac, Android), with native hooks into UNYTE for blockchain testing and ULE-Protocol for decentralization.

In the ULE ecosystem, d30.djs powers dynamic logic in frontend/backend layers, allowing developers to embed UNYSL canisters for smart contract interactions or lofi.css for adaptive UI styling---all within a single file.

## Key Features

- **JavaScript-Like Syntax**: Familiar ES6+ features (async/await, modules, classes) with extensions for blockchain primitives like wallets, transactions, and gas estimation.
- **Embeddable Components**: Seamlessly include UNYSL code blocks for typed logic, lofi.css rules for styling, or even canister calls.
- **Resilient Execution**: Automatic retry mechanisms, circuit breakers, and non-Newtonian-inspired "hardening" for handling spikes in load or errors.
- **State Management**: Built-in persistent storage via Aviyon Cloud integration, with orthogonal persistence similar to UNYSL.
- **Multichain Support**: Via Unyversal SDK, handle cross-chain swaps, bridges, and queries without boilerplate.
- **Serverless Ready**: Deploy to Aviyon Cloud for P2P execution, or run locally with UNYTE for zero-cost testing.
- **Extensible Modules**: Import from npm ecosystem (with ULE-specific wrappers) or ULE-native libraries like ULE-Protocol utilities.

## The ULE Stack Integration

d30.djs is a foundational layer in the ULE Stack, enabling hybrid frontend/backend development:

| Component          | Role with d30.djs                                                      |
|--------------------|------------------------------------------------------------------------|
| **Frontend**       | Embed in `.html.uny` for client-side scripts; pair with lofi.css for dynamic UIs. |
| **Frontend/Backend** | Core runtime for `.djs` files; handles logic, API calls, and UNYSL embeddings. |
| **Database/Nodes** | Integrates with Aviyon Cloud for P2P state persistence and node orchestration. |
| **Blockchain Server** | Uses UNYTE for local testing; deploys canisters via d30.djs scripts. |
| **Infrastructure** | Auto-integrates ULE-Protocol for decentralized routing and liquidity hooks. |
| **Git Integration** | Aviyon Git for versioning `.djs` files alongside UNYSL and lofi.css. |
- **Embeddings Example**: A `.djs` file can contain inline UNYSL for canister logic or lofi.css for styles, reducing context switching.
- **Standalone or Integrated**: Use as a lightweight Node.js alternative or fully embedded in ULE projects.

## d30.djs vs. Other Runtimes

| Feature              | d30.djs (ULE)                | Node.js                      | Deno                         |
|----------------------|------------------------------|------------------------------|------------------------------|
| **Primary Goal**     | Resilient full-stack dApps   | Server-side JavaScript       | Secure modern JS/TS runtime  |
| **Resilience**       | Built-in hardening (retries, breakers) | Requires add-ons (e.g., pm2) | Basic error handling         |
| **Blockchain Integration** | Native (UNYTE, ULE-Protocol) | Via libraries (e.g., ethers) | Via libraries                |
| **Embeddings**       | UNYSL, lofi.css, canisters   | None native                  | None native                  |
| **Persistence**      | Orthogonal via Aviyon Cloud  | Manual (e.g., databases)     | Manual                       |
| **Deployment**       | Serverless P2P or local      | Servers/VMs                  | Edge functions               |

## Why d30.djs?

- **Effortless Blockchain Handling**: Abstracts away "weirdness" like gas fees, nonces, and chain switching---focus on logic.
- **Performance Under Pressure**: Like D30 fluid, it remains "lofi in nature" (simple, efficient) but "hardens & stoic" during spikes, with auto-scaling via Aviyon nodes.
- **Unified Development**: Write once for web/mobile/software; embed other ULE languages for modularity.
- **Cost-Effective**: Local UNYTE nodes for free testing; zero-fee operations on ULE for listings.
- **Security**: Sandboxed execution, type-safe embeddings (via UNYSL), and automatic protocol compliance.

In traditional apps, you'd need separate tools for JS runtime and blockchain bridges. With d30.djs:

| Part of App | Tools                       | Role in ULE                                                          |
|-------------|-----------------------------|----------------------------------------------------------------------|
| **Frontend** | d30.djs + lofi.css         | Dynamic client scripts; reactive UIs with embedded styles.           |
| **Backend** | d30.djs + UNYSL            | Server logic, API endpoints, and persistent state.                   |
| **Bridge**  | UNYTE + Unyversal SDK      | Seamless canister calls and multichain translations.                 |

## Installation

1\. **Via ULE Stack**: Download from [ULE.dev](https://ule.dev) (includes d30.djs pre-bundled).
2\. **NPM Global Install**:

   ```

   npm install -g d30-djs
   d30 --version

   ```

3\. **Project Setup**:

   ```

   npm init d30-project my-app
   cd my-app
   npm install

   ```

For blockchain testing: Install UNYTE as a dependency (`npm i unyte`).

## Getting Started

1\. Create a script:

   ```

   touch hello.djs

   ```

2\. Write basic code (see examples below).
3\. Run locally:

   ```

   d30 run hello.djs

   ```

4\. For blockchain: Start UNYTE node (`npx unyte node`), then run your script with `--network local`.

## Examples

### Basic Hello World (Standalone Script)

```javascript

// hello.djs
console.log('Hello from d30.djs!');
// Embed lofi.css for hypothetical styling (if in a web context)
const styles = `
@lofi-theme {
  --bg-color: #f0f0f0;
}

body { background: var(--bg-color); }
`;

// Async example
async function fetchData() {
  // Simulate API call
  return new Promise(resolve => setTimeout(() => resolve('Data fetched'), 1000));
}

async function main() {
  const data = await fetchData();
  console.log(data);
}

main();

```

Run: `d30 run hello.djs`

### Blockchain Integration (Counter with UNYSL Embedding)

```javascript

// counter.djs
// Embed UNYSL canister logic
const unyslBlock = `
actor Counter {
  var count: Nat = 0;
  public func increment(): async Nat {
    count += 1;
    return count;
  };
}

`;

// Use UNYTE bridge
import { deployCanister, callCanister } from 'unyte';
// Resilient async function with retry
async function incrementWithRetry(maxRetries = 3) {
  let attempts = 0;
  while (attempts < maxRetries) {
    try {
      const result = await callCanister('Counter', 'increment');
      return result;
    } catch (error) {
      attempts++;
      console.warn(`Retry ${attempts}: ${error}`);
      if (attempts === maxRetries) throw error;
    }
  }
}

async function main() {

  // Deploy embedded UNYSL
  await deployCanister(unyslBlock, 'Counter');
  const newCount = await incrementWithRetry();
  console.log(`New count: ${newCount}`);

}

main();

```

This demonstrates embedding UNYSL, calling canisters, and built-in resilience.

### Web Frontend Example (Embedded in .html.uny)

```html

<!-- app.html.uny -->
<!DOCTYPE html>
<html>
<head>
  <!-- Embed lofi.css -->
  <style type="lofi/css">
    button {
      background: #007bff;
      color: white;
    }

  </style>
</head>
<body>
  <button onclick="handleClick()">Click Me</button>
  <!-- Embed d30.djs -->
  <script type="d30/djs">
    async function handleClick() {
      // Embed mini UNYSL for logic
      const unysl = `
      func compute(x: Nat): Nat { x * 2 };
      `;

      // Simulate UNYSL eval (via runtime)
      const result = evalUnysl(unysl, 'compute', 5);
      alert(`Result: ${result}`);

    }

  </script>
</body>
</html>

```

Serve with UNYTE: `npm run dev`

## Advanced Usage

- **Resilience Patterns**:

  ```javascript

  // circuit-breaker.djs
  import { CircuitBreaker } from 'd30/resilience';
  const breaker = new CircuitBreaker({ timeout: 5000, errorThreshold: 50 });
  async function riskyOperation() {
    return breaker.execute(async () => {
      // Potentially failing code
      if (Math.random() > 0.5) throw new Error('Impact!');
      return 'Success';
    });
  }

  ```

- **Multichain Swaps**:

  Use Unyversal SDK for gas-zaps:

  ```javascript

  import { gasZap } from 'unyversal-sdk';
  async function buyNFT(tokenId) {

    // Auto-swap ETH to $ULE if needed
    await gasZap('ETH', '$ULE', async (uleAmount) => {
      // Execute transaction on ULE
      console.log(`Bought NFT ${tokenId} with ${uleAmount} $ULE`);
    });

  }

  ```

- **P2P Deployment**: Push to Aviyon Cloud:

  ```

  d30 deploy --cloud aviyon my-script.djs

  ```

## Performance and Resilience

- **Benchmarking**: d30.djs achieves Node.js-level throughput with 20-30% better error recovery in stress tests (e.g., 10k concurrent requests).
- **Hardening Mechanisms**: Auto-throttling, memory hardening during GC pressure, and fluid scaling across Aviyon nodes.
- **Metrics**: Integrate with ULE monitoring for real-time dashboards on gas usage, latency, and impact events.

## Development Workflow

- **Local**: Run scripts with `d30 run`; test blockchain with UNYTE.
- **Editors**: VS Code with d30 extension for syntax highlighting and embeddings.
- **CI/CD**: Aviyon Git for automated deploys to P2P networks.
- **Tools**: Oxygen-CLI for terminal scripting; Studio for visual debugging.

## The ULE Ecosystem

d30.djs thrives in the ULE ecosystem:

- **ULE Network**: Layer 1 with $ULE as native gas.
- **ULE-Protocol**: Liquidity engine with ULPs and cross-chain routing.
- **Unyversal SDK**: Translator for multichain ops.
- **UnySON/UnyFi**: Ecosystem connectors and distro programs.
- **Validators**: Meet hardware specs for staking $ULE.

Flywheel: d30.djs apps drive $ULE usage, burns, and network growth.

## Contributing

Fork, PR, discuss on [Discord](https://discord.gg/d30djs). See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

MIT License - see [LICENSE](LICENSE).
