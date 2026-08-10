---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: briskhealthurgentcare.com
  spf: false
- caa: []
  dmarc: true
  dmarc_note: Two conflicting DMARC TXT records are published at _dmarc.briskhealth.com — one "p=none" carrying unedited template placeholders (rua/ruf pointing at dmarc-reports@yourdomain.com) and one "p=reject". Per RFC 7489 6.6.3 a receiver that finds more than one DMARC record discards the policy entirely, so this domain is effectively unprotected despite appearing to publish a reject policy.
  dmarc_policy: invalid-multiple-records
  dnssec: false
  domain: briskhealth.com
  spf: true
  spf_record: v=spf1 include:_spf.mlsend.com include:_spf.enguard.com -all
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brisk.health
  spf: true
  spf_record: v=spf1 include:_spf.google.com ~all
hosts:
- cert_expires: Sep  6 01:16:14 2026 GMT
  cert_valid: true
  host: www.briskhealthurgentcare.com
  hsts: true
  hsts_max_age: 31556952
  http_status: 200
  https: true
  role: live marketing site (only reachable Brisk Health web property)
  tls_version: TLSv1.3
- cert_expires: Oct 28 11:02:37 2026 GMT
  cert_valid: true
  host: briskhealth.com
  hsts: false
  http_body: Wix "ConnectYourDomain Error" page
  http_status: 404
  https: true
  role: primary brand domain — parked / misconfigured
  tls_version: TLSv1.3
- cert_expires: Mar 27 05:04:50 2026 GMT
  cert_note: Certificate expired 2026-03-27 and has not been renewed; a default TLS client refuses the connection outright.
  cert_valid: false
  host: brisk.health
  hsts: false
  http_body: Wix "ConnectYourDomain Error" page
  http_status: 404
  https: true
  role: mobile-app landing domain (linked from the marketing site) — dead
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brisk Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brisk Health, probed live across 3 host(s) and 3 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Brisk Health
provider_slug: brisk-health
slug: brisk-health-domain-security
source_filename: brisk-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every Brisk Health host found during enrichment\nnote: >-\n  Scoped to domains Brisk Health controls. The mechanical probe also walked\n  dev.wix.com / wix.com because the Wix Site MCP documentation is the only human\n  URL for the site's MCP surface; those are Wix's domains, not Brisk Health's, and\n  have been removed so this artifact describes only the provider.\nhosts:\n- host: www.briskhealthurgentcare.com\n  role: live marketing site (only reachable Brisk Health web property)\n  http_status: 200\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 01:16:14 2026 GMT\n  cert_valid: true\n  hsts: true\n  hsts_max_age: 31556952\n- host: briskhealth.com\n  role: primary brand domain — parked / misconfigured\n  http_status: 404\n  http_body: Wix \"ConnectYourDomain Error\" page\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 11:02:37 2026 GMT\n  cert_valid: true\n  hsts: false\n\
  - host: brisk.health\n  role: mobile-app landing domain (linked from the marketing site) — dead\n  http_status: 404\n  http_body: Wix \"ConnectYourDomain Error\" page\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 05:04:50 2026 GMT\n  cert_valid: false\n  cert_note: >-\n    Certificate expired 2026-03-27 and has not been renewed; a default TLS client\n    refuses the connection outright.\n  hsts: false\ndomains:\n- domain: briskhealthurgentcare.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: briskhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.mlsend.com include:_spf.enguard.com -all\n  dmarc: true\n  dmarc_policy: invalid-multiple-records\n  dmarc_note: >-\n    Two conflicting DMARC TXT records are published at _dmarc.briskhealth.com —\n    one \"p=none\" carrying unedited template placeholders\n    (rua/ruf pointing at dmarc-reports@yourdomain.com) and one \"p=reject\". Per\n    RFC 7489 6.6.3 a receiver that\
  \ finds more than one DMARC record discards the\n    policy entirely, so this domain is effectively unprotected despite appearing\n    to publish a reject policy.\n- domain: brisk.health\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com ~all\n  dmarc: true\n  dmarc_policy: none\nfindings:\n- id: expired-tls-cert\n  host: brisk.health\n  severity: high\n  detail: TLS certificate expired 2026-03-27; the app landing domain is unusable over HTTPS.\n- id: dmarc-multiple-records\n  domain: briskhealth.com\n  severity: medium\n  detail: Duplicate DMARC records void the policy; one still contains template placeholders.\n- id: no-caa\n  severity: low\n  detail: No CAA records on any Brisk Health domain, so certificate issuance is unrestricted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brisk-health/refs/heads/main/security/brisk-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Urgent Care
- Primary Care
- Home Health
- Clinics
- Colorado
---
