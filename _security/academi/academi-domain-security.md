---
description: ''
domains:
- caa: []
  created: '1999-08-04'
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1;p=reject;sp=reject;pct=100;rua=mailto:itsec@constellis.com;fo=1
  dnssec: true
  domain: academi.com
  expires: '2027-08-04'
  mx:
  - mxa-004a2a01.gslb.pphosted.com
  - mxb-004a2a01.gslb.pphosted.com
  nameservers: AWS Route 53
  note: Registered and actively maintained, but web-retired. The DMARC rua address itsec@constellis.com is first-party evidence that the acquirer administers this domain.
  registrar: Tucows Domains Inc.
  spf: true
  spf_record: v=spf1 include:spf-004a2a01.pphosted.com -all
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: constellis.com
  spf: true
hosts:
- cert_expires: null
  host: academi.com
  hsts: false
  https: false
  note: 'TLS handshake failure on 443 (no certificate covering the hostname). Port 80 answers HTTP 409 with a Cloudflare "error code: 1001" body on every path, including the apex - an unconfigured-host response. No HSTS because there is no HTTPS response.'
  tls_version: null
- cert_expires: Oct 10 00:02:12 2026 GMT
  host: constellis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Academi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Academi, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Academi
provider_slug: academi
slug: academi-domain-security
source_filename: academi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts (constellis.com, the successor host wired\n  as this record's Website pointer), plus a hand-run probe of Academi's own domain academi.com, which\n  carries no Website pointer because it serves no site\nhosts:\n- host: academi.com\n  https: false\n  tls_version: null\n  cert_expires: null\n  hsts: false\n  note: 'TLS handshake failure on 443 (no certificate covering the hostname). Port 80 answers HTTP 409\n    with a Cloudflare \"error code: 1001\" body on every path, including the apex - an unconfigured-host\n    response. No HSTS because there is no HTTPS response.'\n- host: constellis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 00:02:12 2026 GMT\n  hsts: false\ndomains:\n- domain: academi.com\n  dnssec: true\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf-004a2a01.pphosted.com -all\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: v=DMARC1;p=reject;sp=reject;pct=100;rua=mailto:itsec@constellis.com;fo=1\n\
  \  mx:\n  - mxa-004a2a01.gslb.pphosted.com\n  - mxb-004a2a01.gslb.pphosted.com\n  nameservers: AWS Route 53\n  registrar: Tucows Domains Inc.\n  created: '1999-08-04'\n  expires: '2027-08-04'\n  note: Registered and actively maintained, but web-retired. The DMARC rua address itsec@constellis.com\n    is first-party evidence that the acquirer administers this domain.\n- domain: constellis.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nnote: 'academi.com is the subject domain and is recorded first. It has NO working HTTPS listener - the\n  TLS handshake on port 443 fails outright - while its DNS is fully maintained: DNSSEC signed, Proofpoint\n  MX, an SPF record and a DMARC record at p=reject whose aggregate reports go to itsec@constellis.com.\n  That is a mail-retained, web-retired domain administered by the acquirer. constellis.com is the successor\n  operator''s host and its posture is Constellis'', not Academi''s.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/academi/refs/heads/main/security/academi-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Defense
- Private Military
- Security Services
- Physical Security
- Training
- Government Contracting
- Logistics
- Program Management
- Acquired
- Brand Retired
---
