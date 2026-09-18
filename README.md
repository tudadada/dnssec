# dnssec

[![npm version](https://img.shields.io/npm/v/dnssec.svg)](https://www.npmjs.com/package/dnssec)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

**Domain Name System Security Extensions (DNSSEC)** MCP Server. Real-time cryptographic validation of DNS root-to-leaf trust chains, RRSIG expiration audits, and automated DNS spoofing defense for AI agents.

## Features

- **Chain of Trust Verification**: Recursive validation spanning ICANN Root, TLD, and authoritative zone keys.
- **Record Auditing**: Automated inspection of DNSKEY, DS, and RRSIG signature parameters.
- **Model Context Protocol (MCP)**: Native integration for AI coding assistants and autonomous agent workflows.

## Quick Start

### Direct Execution
```bash
npx dnssec
```

### Claude Desktop Integration

Add to your `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "dnssec": {
      "command": "npx",
      "args": ["-y", "dnssec"]
    }
  }
}
```

## Tools Included

1. `verify_dnssec_chain`: Validates cryptographic chain of trust and detects spoofing/tampering.
2. `audit_dnssec_records`: Checks cipher strength, key tags, and signature expiration dates.

## License

MIT © [tudadada](https://github.com/tudadada)
