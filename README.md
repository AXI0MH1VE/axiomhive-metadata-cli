# AxiomHive Metadata CLI

> **User Sovereignty Enforced:** All authentication local, all commands transparent and auditable.

GitHub CLI automation tool for batch metadata updates across AxiomHive repositories. This tool enables systematic updates to repository descriptions, homepage URLs, and topics while maintaining complete user control over execution.

---

## Constitutional Framework

![CDA Compliant](https://img.shields.io/badge/CDA-v1.0%20Compliant-brightgreen)
[![Constitution](https://img.shields.io/badge/Constitution-Read-blue)](https://github.com/AXI0MH1VE/CDA-Constitution)

This project operates under the **[Constitution of a Deterministic Assistant (CDA-v1.0)](https://github.com/AXI0MH1VE/CDA-Constitution)**.

**Core Principles:**
- 🔍 **Transparency**: All commands auditable - no hidden operations
- ⚙️ **Determinism**: User-initiated actions only - no autonomous behavior
- 🤝 **Subservience**: Complete user control - local authentication enforced

See [.github/CONSTITUTION.md](.github/CONSTITUTION.md) for full constitutional text.

---

## ⚠️ Security & Sovereignty

### **Critical Principle: You Are the Single Source of Truth**

- **No agent executes this script**
- **No remote automation**
- **Uses YOUR local `gh` CLI authentication**
- **All commands are human-readable and auditable**
- **You review and execute locally**

## Prerequisites

### Required
- [GitHub CLI (`gh`)](https://cli.github.com/) installed
- Authenticated GitHub account with write access to AXI0MH1VE repositories

### Installation

```bash
# Install GitHub CLI (if not installed)
# macOS
brew install gh

# Windows
winget install --id GitHub.cli

# Linux
# See: https://github.com/cli/cli/blob/trunk/docs/install_linux.md

# Authenticate
gh auth login
```

## Usage

### 1. Clone this repository

```bash
git clone https://github.com/AXI0MH1VE/axiomhive-metadata-cli.git
cd axiomhive-metadata-cli
```

### 2. Make the script executable

```bash
chmod +x update_metadata.sh
```

### 3. Review the script (IMPORTANT)

```bash
cat update_metadata.sh  # Review all commands before execution
```

### 4. Execute

```bash
./update_metadata.sh
```

## What It Does

The script updates metadata for 30+ AxiomHive repositories:

- **Description:** Sets clear, deterministic AI-focused descriptions
- **Homepage:** Sets to https://axiomhive.org
- **Topics:** Adds relevant tags (deterministic-ai, safety-critical, rust, python, etc.)

### Repository Categories

- **Core Infrastructure:** Matrix-42, Hydra7N, axiomhive-evidence-framework
- **AI Frameworks:** AxiomHive-Phoenix, ACE-AGI, OmniCrush
- **Utilities:** DEVDOLLZ, ARTIFACTS, GeminiPortable

## Expanding Coverage

The current script covers 30 repositories. To add more:

1. Use the `update_repo` function pattern:

```bash
update_repo "repo-name" "Description" "topic1" "topic2" "topic3" "topic4" "topic5"
```

2. Categories are separated by comments for organization
3. Keep topics focused on deterministic AI positioning

## Verification

After execution, verify updates:

```bash
# Check a specific repository
gh repo view AXI0MH1VE/Matrix-42

# Or visit the repository pages
```

## Architecture Principles

### Deterministic AI Positioning

All repository metadata emphasizes:
- **Mathematical provability**
- **Formal verification**
- **Zero-entropy guarantees**
- **Safety-critical applications**
- **Cryptographic integrity**

### Topic Strategy

Core topics applied across repos:
- `deterministic-ai` - Primary identifier
- `safety-critical` - High-stakes applications
- `formal-verification` - Mathematical proofs
- `rust` / `python` - Implementation languages
- `cryptography` - Cryptographic guarantees

## Repository Structure

```
axiomhive-metadata-cli/
├── README.md              # This file
├── LICENSE                # MIT License
├── update_metadata.sh     # Main automation script
└── .gitignore             # Git exclusions
```

## Troubleshooting

### Authentication Issues

```bash
# Check authentication status
gh auth status

# Re-authenticate if needed
gh auth login
```

### Permission Errors

- Ensure you have write access to AXI0MH1VE repositories
- Verify organization membership if applicable

### Script Execution Errors

```bash
# Make script executable
chmod +x update_metadata.sh

# Run with bash explicitly
bash update_metadata.sh
```

## Contributing

To add more repositories to the update script:

1. Fork this repository
2. Add `update_repo` calls following the existing pattern
3. Test locally with `--dry-run` (if implementing)
4. Submit a pull request

## License

MIT License - See [LICENSE](LICENSE) file

## Author

**Alexis M. Adams (AXI0MH1VE)**  
Founder & CEO, AxiomHive  
Specializing in Deterministic AI for Safety-Critical Applications

## Related

- [AxiomHive Website](https://axiomhive.org)
- [GitHub Profile](https://github.com/AXI0MH1VE)
- [Deterministic AI Whitepaper](https://github.com/AXI0MH1VE/deterministic-ai-gaslighting-to-guarantees)

---

**⚡ User Sovereignty Enforced**  
*This tool operates exclusively under your local control. No external automation. No agent execution.*