---
api_specs:
- filename: checkpoint-access-rules-api-openapi.yml
  format: yaml
  label: Check Point Access Rules API
  slug: checkpoint-access-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-access-rules-api-openapi.yml
- filename: checkpoint-cloud-accounts-api-openapi.yml
  format: yaml
  label: Check Point Cloud Accounts API
  slug: checkpoint-cloud-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-cloud-accounts-api-openapi.yml
- filename: checkpoint-compliance-api-openapi.yml
  format: yaml
  label: Check Point Compliance API
  slug: checkpoint-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-compliance-api-openapi.yml
- filename: checkpoint-events-api-openapi.yml
  format: yaml
  label: Check Point Events API
  slug: checkpoint-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-events-api-openapi.yml
- filename: checkpoint-findings-api-openapi.yml
  format: yaml
  label: Check Point Findings API
  slug: checkpoint-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-findings-api-openapi.yml
- filename: checkpoint-hosts-api-openapi.yml
  format: yaml
  label: Check Point Hosts API
  slug: checkpoint-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-hosts-api-openapi.yml
- filename: checkpoint-identity-api-openapi.yml
  format: yaml
  label: Check Point Identity API
  slug: checkpoint-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-identity-api-openapi.yml
- filename: checkpoint-interfaces-api-openapi.yml
  format: yaml
  label: Check Point Interfaces API
  slug: checkpoint-interfaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-interfaces-api-openapi.yml
- filename: checkpoint-login-api-openapi.yml
  format: yaml
  label: Check Point Login API
  slug: checkpoint-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-login-api-openapi.yml
- filename: checkpoint-nat-rules-api-openapi.yml
  format: yaml
  label: Check Point NAT Rules API
  slug: checkpoint-nat-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-nat-rules-api-openapi.yml
- filename: checkpoint-networks-api-openapi.yml
  format: yaml
  label: Check Point Networks API
  slug: checkpoint-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-networks-api-openapi.yml
- filename: checkpoint-quarantine-api-openapi.yml
  format: yaml
  label: Check Point Quarantine API
  slug: checkpoint-quarantine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-quarantine-api-openapi.yml
- filename: checkpoint-routes-api-openapi.yml
  format: yaml
  label: Check Point Routes API
  slug: checkpoint-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-routes-api-openapi.yml
- filename: checkpoint-rulesets-api-openapi.yml
  format: yaml
  label: Check Point Rulesets API
  slug: checkpoint-rulesets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-rulesets-api-openapi.yml
- filename: checkpoint-services-api-openapi.yml
  format: yaml
  label: Check Point Services API
  slug: checkpoint-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-services-api-openapi.yml
- filename: checkpoint-sessions-api-openapi.yml
  format: yaml
  label: Check Point Sessions API
  slug: checkpoint-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-sessions-api-openapi.yml
- filename: checkpoint-system-api-openapi.yml
  format: yaml
  label: Check Point System API
  slug: checkpoint-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-system-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:hostmaster@checkpoint.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: checkpoint.com
  spf: true
hosts:
- cert_expires: Jan  2 06:44:08 2027 GMT
  host: www.checkpoint.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: sc1.checkpoint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 09:25:52 2026 GMT
  host: docs.cgn.portal.checkpoint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Checkpoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Check Point, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Check Point
provider_slug: checkpoint
slug: checkpoint-domain-security
source_filename: checkpoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.checkpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 06:44:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: sc1.checkpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: false\n- host: docs.cgn.portal.checkpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 09:25:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: checkpoint.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:hostmaster@checkpoint.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/security/checkpoint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cloud Security
- Cybersecurity
- Endpoint Security
- Firewall
- Identity Awareness
- Mobile Security
- Network Security
- Security
- Threat Prevention
- WAF
---
