#!/bin/bash

# Create the docs folder if it doesn't exist
mkdir -p docs

# Create or overwrite architecture.md
cat <<'EOF' > docs/architecture.md
# Architecture

This document outlines the overall architecture of NadoxDocumentation. It describes the cloud-powered API system, the underlying backend technologies, and the integration with modern cloud services. The design emphasizes modularity, high performance, and scalability.

**Key Components:**
- **Cloud API:** Uses AWS Lambda, API Gateway, and CloudFront.
- **Modular Structure:** Separates documentation, source code, and tests.
- **Integration:** Connects backend services with open-source tools.
EOF

# Create or overwrite setup.md
cat <<'EOF' > docs/setup.md
# Setup Guide

This guide provides step-by-step instructions to set up NadoxDocumentation on your local machine or server.

**Prerequisites:**
- Git installed
- Configured cloud environment (e.g., AWS)
- Familiarity with backend development

**Installation Steps:**
1. Clone the repository:
   ```bash
   git clone git@github.com:timedilationv2/nadoxdocumentation.git
   cd nadoxdocumentation
