---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: proxykey.org
  spf: false
hosts:
- cert_expires: Dec  1 18:52:15 2026 GMT
  host: proxykey.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Proxykey Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for proxykey-org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: proxykey-org
provider_slug: proxykey-org
slug: proxykey-org-domain-security
source_filename: proxykey-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: proxykey.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 18:52:15 2026 GMT\n  hsts: false\ndomains:\n- domain: proxykey.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/proxykey-org/security/proxykey-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Security
- API-Management
- Encryption
- Key-Vault
- Developer-Tools
---
