---
api_specs:
- filename: california-attorney-general-openjustice-jsonapi-openapi.yml
  format: yaml
  label: OpenJustice Open Data Portal JSON:API
  slug: openjustice-open-data-portal-jsonapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/california-attorney-general/refs/heads/main/openapi/california-attorney-general-openjustice-jsonapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1;p=quarantine;rua=mailto:dojdmarcrua@doj.ca.gov;ruf=mailto:dojdmarcruf@doj.ca.gov;fo=1
  dnssec: false
  dnssec_note: no DS record and no RRSIG on the A answer
  domain: oag.ca.gov
  spf: true
  spf_record: v=spf1 a mx include:public.govdelivery.com -all
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1;p=quarantine;rua=mailto:dojdmarcrua@doj.ca.gov;ruf=mailto:dojdmarcruf@doj.ca.gov;fo=1
  dnssec: false
  domain: doj.ca.gov
  spf: true
  spf_record: v=spf1 ip4:167.10.243.94 ip4:167.10.240.132 ip4:167.10.240.129 ip4:167.10.240.1 include:spf-00292801.pphosted.com include:_phishspf.knowbe4.com include:spf.protection.outlook.com include:spf-00292802.pphosted.com -all
- caa: []
  credited: false
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ca.gov
  note: Shared State of California domain (Department of Technology) — recorded for reference only.
  spf: true
hosts:
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: oag.ca.gov
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: openjustice.doj.ca.gov
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: data-openjustice.doj.ca.gov
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: California Attorney General Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for California Attorney General, probed live across 3 host(s) and 3 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: California Attorney General
provider_slug: california-attorney-general
slug: california-attorney-general-domain-security
source_filename: california-attorney-general-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts on 2026-09-17; domain records re-probed by hand with\n  dig against the AG/DOJ zones (oag.ca.gov, doj.ca.gov) rather than the shared state domain ca.gov\nhosts:\n- host: oag.ca.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: false\n- host: openjustice.doj.ca.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\n- host: data-openjustice.doj.ca.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: oag.ca.gov\n  dnssec: false\n  dnssec_note: no DS record and no RRSIG on the A answer\n  caa: []\n  spf: true\n  spf_record: v=spf1 a mx include:public.govdelivery.com -all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: v=DMARC1;p=quarantine;rua=mailto:dojdmarcrua@doj.ca.gov;ruf=mailto:dojdmarcruf@doj.ca.gov;fo=1\n\
  - domain: doj.ca.gov\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 ip4:167.10.243.94 ip4:167.10.240.132 ip4:167.10.240.129 ip4:167.10.240.1 include:spf-00292801.pphosted.com\n    include:_phishspf.knowbe4.com include:spf.protection.outlook.com include:spf-00292802.pphosted.com -all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: v=DMARC1;p=quarantine;rua=mailto:dojdmarcrua@doj.ca.gov;ruf=mailto:dojdmarcruf@doj.ca.gov;fo=1\n- domain: ca.gov\n  credited: false\n  note: Shared State of California domain (Department of Technology) — recorded for reference only.\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nnote: The registrable-domain heuristic resolves oag.ca.gov to ca.gov, which is the State of California's shared\n  portal domain operated by the Department of Technology, not the Attorney General's. The `domains` block below\n  therefore records oag.ca.gov and doj.ca.gov, the zones the DOJ itself runs (its DMARC reports go to dojdmarcrua@doj.ca.gov).\n\
  \  ca.gov is listed last for reference only and is NOT credited to this provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/california-attorney-general/refs/heads/main/security/california-attorney-general-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- State-Government
- California
- Criminal Justice
- Open Data
- Law Enforcement
- Crime Statistics
- Government Data
- JSON:API
- Public Records
- Attorney General
---
