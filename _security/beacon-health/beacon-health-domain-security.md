---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: beaconhealth.ai
  spf: false
hosts:
- cert_expires: Nov 10 09:56:16 2026 GMT
  host: www.beaconhealth.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 14:31:22 2026 GMT
  host: api.beaconhealth.ai
  hsts: false
  hsts_max_age: null
  https: true
  note: No Strict-Transport-Security header on either the 404 root or the 200 /.well-known/openid-configuration response. Fronted by Cloudflare.
  role: application backend (Convex); serves OIDC discovery + JWKS
  tls_version: TLSv1.3
- cert_expires: Oct 19 02:54:49 2026 GMT
  host: trust.beaconhealth.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: trust center (Oneleet)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beacon Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beacon Health, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Beacon Health
provider_slug: beacon-health
slug: beacon-health-domain-security
source_filename: beacon-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  www.beaconhealth.ai is probed mechanically by 0-working/probe-domain-security.py\n  from apis.yml. The api. and trust. hosts are not named in apis.yml (there is no\n  API entry), so they were probed by hand on the same date with the same method —\n  openssl s_client for TLS/cert, HTTP HEAD for HSTS.\nhosts:\n- host: www.beaconhealth.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 09:56:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.beaconhealth.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 14:31:22 2026 GMT\n  hsts: false\n  hsts_max_age: null\n  role: application backend (Convex); serves OIDC discovery + JWKS\n  note: >-\n    No Strict-Transport-Security header on either the 404 root or the 200\n    /.well-known/openid-configuration response. Fronted by Cloudflare.\n- host: trust.beaconhealth.ai\n  https:\
  \ true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 02:54:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  role: trust center (Oneleet)\ndomains:\n- domain: beaconhealth.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beacon-health/refs/heads/main/security/beacon-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Primary Care
- Value Based Care
- EHR
- Artificial Intelligence
- AI Agents
- Workflow Automation
- Risk Adjustment
- Prior Authorization
- HIPAA
- Y Combinator
---
