---
api_specs:
- filename: jama-software-openapi-generated.yml
  format: yaml
  label: Jama Connect REST API
  slug: jama-connect-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jama-software/refs/heads/main/openapi/_ae-authored/jama-software-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jamasoftware.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: jamacloud.com
  spf: true
hosts:
- cert_expires: Dec 17 13:46:43 2026 GMT
  host: www.jamasoftware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 19:20:33 2027 GMT
  host: rest.jamasoftware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: tenant.jamacloud.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Jama Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jama Software, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jama Software
provider_slug: jama-software
slug: jama-software-domain-security
source_filename: jama-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jamasoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 13:46:43 2026 GMT\n  hsts: false\n- host: rest.jamasoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 19:20:33 2027 GMT\n  hsts: false\n- host: tenant.jamacloud.com\n  https: false\ndomains:\n- domain: jamasoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: jamacloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jama-software/refs/heads/main/security/jama-software-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Requirements Management
- Application Lifecycle Management
- Traceability
- Test Management
- Product Development
- Systems Engineering
- REST API
---
