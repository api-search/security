---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Sigstore Rekor API (consumed)
  slug: rekor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/sigstore/rekor/main/openapi.yaml
- filename: fulcio.swagger.json
  format: json
  label: Sigstore Fulcio API (consumed)
  slug: fulcio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/sigstore/fulcio/main/fulcio.swagger.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@sigstore.dev"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sigstore.dev
  spf: true
hosts:
- cert_expires: Oct 10 23:23:48 2026 GMT
  host: www.sigstore.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:13:41 2026 GMT
  host: docs.sigstore.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 12:11:57 2026 GMT
  host: rekor.sigstore.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Cosign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cosign, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cosign
provider_slug: cosign
slug: cosign-domain-security
source_filename: cosign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sigstore.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:23:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sigstore.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:13:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rekor.sigstore.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 12:11:57 2026 GMT\n  hsts: false\ndomains:\n- domain: sigstore.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@sigstore.dev\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosign/refs/heads/main/security/cosign-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apache 2.0
- Attestations
- CLI
- Code Signing
- Containers
- Fulcio
- Go
- Keyless
- OCI
- OIDC
- Open-Source
- Rekor
- Sigstore
- Supply Chain
- Transparency Log
- Verification
---
