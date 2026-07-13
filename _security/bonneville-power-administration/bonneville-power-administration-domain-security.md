---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issue "identrust.com"
  - 0 issue "entrust.net"
  - 0 iodef "mailto:dns-admin@bpa.gov"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bpa.gov
  spf: true
- caa:
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:vkeymaster@esri.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arcgis.com
  spf: true
hosts:
- cert_expires: Mar 21 22:16:52 2027 GMT
  host: www.bpa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: data-bpagis.hub.arcgis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 18:37:22 2027 GMT
  host: transmission.bpa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bonneville Power Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bonneville Power Administration, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bonneville Power Administration
provider_slug: bonneville-power-administration
slug: bonneville-power-administration-domain-security
source_filename: bonneville-power-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bpa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 21 22:16:52 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data-bpagis.hub.arcgis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: transmission.bpa.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 13 18:37:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bpa.gov\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issue \"identrust.com\"\n  - 0 issue \"entrust.net\"\n  - 0 iodef \"mailto:dns-admin@bpa.gov\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: arcgis.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:vkeymaster@esri.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue\
  \ \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonneville-power-administration/refs/heads/main/security/bonneville-power-administration-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Federal Government
- GIS
- Hydroelectric
- Pacific Northwest
- Power
- Transmission
- Wind
---
