---
description: TLS, HSTS and DNS posture across every Tava Health host found in this pass. All four hosts serve TLS 1.3 with valid certificates and HSTS at a one-year max-age; the two portal hosts additionally set includeSubDomains. At the DNS layer tavahealth.com publishes SPF and a DMARC policy of quarantine but has no DNSSEC and no CAA record — both are absences, recorded as observed rather than inferred.
domains:
- caa: []
  caa_note: No CAA record published; any CA may issue for this domain.
  dmarc: true
  dmarc_note: Policy p=quarantine — deployed and enforcing, short of p=reject.
  dmarc_policy: quarantine
  dnssec: false
  dnssec_note: No DNSKEY record — the zone is not signed.
  domain: tavahealth.com
  spf: true
hosts:
- cert_expires: Oct 15 08:32:09 2026 GMT
  host: www.tavahealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Marketing site (Webflow).
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: care.tavahealth.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Client (member) portal. Static single-page app served from S3; catch-all route answers 200 for every path.
  server: AmazonS3
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: app.tavahealth.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Provider/administrative portal ("Harmony"). Static single-page app served from S3.
  server: AmazonS3
  tls_version: TLSv1.3
- cert_expires: Nov 18 18:57:58 2026 GMT
  host: docs.tavahealth.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  https: true
  note: DirectCare developer hub on ReadMe.io behind Cloudflare. Password-gated; sets x-frame-options Deny, x-content-type-options nosniff, and a 100-request rate limit header.
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tava Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tava Health, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tava Health
provider_slug: tava-health
slug: tava-health-domain-security
source_filename: tava-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts, extended by hand to the three additional Tava Health\n  hosts discovered during contract discovery (client portal, provider portal, developer hub)\nhosts:\n- host: www.tavahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 08:32:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: Marketing site (Webflow).\n- host: care.tavahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  server: AmazonS3\n  note: Client (member) portal. Static single-page app served from S3; catch-all route answers 200 for\n    every path.\n- host: app.tavahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  server: AmazonS3\n  note: Provider/administrative\
  \ portal (\"Harmony\"). Static single-page app served from S3.\n- host: docs.tavahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 18:57:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\n  server: cloudflare\n  note: DirectCare developer hub on ReadMe.io behind Cloudflare. Password-gated; sets x-frame-options\n    Deny, x-content-type-options nosniff, and a 100-request rate limit header.\ndomains:\n- domain: tavahealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dnssec_note: No DNSKEY record — the zone is not signed.\n  caa_note: No CAA record published; any CA may issue for this domain.\n  dmarc_note: Policy p=quarantine — deployed and enforcing, short of p=reject.\nname: Tava Health domain security\ndescription: TLS, HSTS and DNS posture across every Tava Health host found in this pass. All four hosts\n  serve TLS 1.3 with valid certificates and HSTS at a one-year max-age; the\
  \ two portal hosts additionally\n  set includeSubDomains. At the DNS layer tavahealth.com publishes SPF and a DMARC policy of quarantine\n  but has no DNSSEC and no CAA record — both are absences, recorded as observed rather than inferred.\nhosts_probed: 4\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tava-health/refs/heads/main/security/tava-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Care
- Mental Health
- Behavioral Health
- Telehealth
- Employee Benefits
- Health Plans
- HIPAA
- Digital Health
- Care Delivery
---
