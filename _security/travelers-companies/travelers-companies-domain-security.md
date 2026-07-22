---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: travelers.com
  spf: true
hosts:
- cert_expires: Aug 14 03:07:59 2026 GMT
  host: www.travelers.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Travelers Companies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Travelers Companies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Travelers Companies
provider_slug: travelers-companies
slug: travelers-companies-domain-security
source_filename: travelers-companies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.travelers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:07:59 2026 GMT\n  hsts: false\ndomains:\n- domain: travelers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travelers-companies/refs/heads/main/security/travelers-companies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Agency Distribution
- Auto Insurance
- Bond and Specialty
- Business Insurance
- Claims
- Commercial Insurance
- Cyber Insurance
- Dow Jones Industrial Average
- Fortune 100
- Homeowners
- Insurance
- Personal Insurance
- Property and Casualty
- Risk Management
- Surety Bonds
- Telematics
- Workers Compensation
---
