---
api_specs:
- filename: misp-openapi-generated.yml
  format: yaml
  label: MISP API
  slug: misp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/misp/refs/heads/main/openapi/_ae-authored/misp-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: misp-project.org
  spf: true
hosts:
- cert_expires: Dec 14 02:51:18 2026 GMT
  host: www.misp-project.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Misp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MISP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: MISP
provider_slug: misp
slug: misp-domain-security
source_filename: misp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.misp-project.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 02:51:18 2026 GMT\n  hsts: false\ndomains:\n- domain: misp-project.org\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/misp/refs/heads/main/security/misp-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- OpenSource
- ThreatIntelligence
- Community
- Security
- Collaboration
- Company
---
