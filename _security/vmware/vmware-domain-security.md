---
api_specs:
- filename: vmware-vsphere-api-openapi.yml
  format: yaml
  label: vSphere API
  slug: vsphere-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-vsphere-api-openapi.yml
- filename: openapi.yaml
  format: yaml
  label: vCloud Director API
  slug: vcloud-director-api
  spec_type: OpenAPI
  url: https://developer.vmware.com/apis/vmware-cloud-director/latest/openapi/
- filename: openapi.yaml
  format: yaml
  label: NSX-T Data Center API
  slug: nsx-t-data-center-api
  spec_type: OpenAPI
  url: https://developer.vmware.com/apis/nsx-t/latest/openapi/
- filename: openapi.yaml
  format: yaml
  label: vRealize Automation API
  slug: vrealize-automation-api
  spec_type: OpenAPI
  url: https://developer.vmware.com/apis/vrealize-automation/latest/openapi/
- filename: openapi.yaml
  format: yaml
  label: VMware Cloud on AWS API
  slug: vmware-cloud-on-aws-api
  spec_type: OpenAPI
  url: https://developer.vmware.com/apis/vmc/latest/openapi/
- filename: openapi.yaml
  format: yaml
  label: vRealize Operations API
  slug: vrealize-operations-api
  spec_type: OpenAPI
  url: https://developer.vmware.com/apis/vrealize-operations/latest/openapi/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: broadcom.com
  spf: true
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "entrust.net"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vmware.com
  spf: true
hosts:
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: developer.broadcom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: developer.vmware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: vmc.vmware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vmware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VMware, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: VMware
provider_slug: vmware
slug: vmware-domain-security
source_filename: vmware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.broadcom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.vmware.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: vmc.vmware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: broadcom.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: vmware.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"entrust.net\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/security/vmware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
---
