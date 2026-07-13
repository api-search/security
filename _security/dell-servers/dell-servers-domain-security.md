---
api_specs:
- filename: dell-servers-idrac-redfish-openapi.yml
  format: yaml
  label: Dell iDRAC Redfish REST API
  slug: dell-servers-idrac-redfish
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-idrac-redfish-openapi.yml
- filename: dell-servers-openmanage-enterprise-openapi.yml
  format: yaml
  label: Dell OpenManage Enterprise API
  slug: dell-servers-openmanage-enterprise
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-openmanage-enterprise-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "pkiadmin@dell.com"
  - 0 iodef "mailto:pkiadmin@dell.com"
  - 0 issue "digicert.com; account=b34fd286db03ccad020f0a75010dd75544eaf2b967195b4becb6460c924d35c9"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dell.com
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: developer.dell.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.dell.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dell Servers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dell Servers, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dell Servers
provider_slug: dell-servers
slug: dell-servers-domain-security
source_filename: dell-servers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.dell.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: www.dell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: dell.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"pkiadmin@dell.com\"\n  - 0 iodef \"mailto:pkiadmin@dell.com\"\n  - 0 issue \"digicert.com; account=b34fd286db03ccad020f0a75010dd75544eaf2b967195b4becb6460c924d35c9\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/security/dell-servers-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Hardware
- Infrastructure
- Management
- Monitoring
- Servers
---
