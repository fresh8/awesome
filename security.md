# Security <!-- omit in toc -->

Security is banging!

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [Education](#education)
    - [Secure Development Processes](#secure-development-processes)
    - [Awareness of Security Risks](#awareness-of-security-risks)
    - [Vulnerable Target Testing](#vulnerable-target-testing)
- [Tools and Resources](#tools-and-resources)
    - [Application Testing Tools](#application-testing-tools)
        - [SAST (Static Application Security Testing)](#sast-static-application-security-testing)
        - [DAST (Dynamic Application Security Testing)](#dast-dynamic-application-security-testing)
        - [IAST (Interactive Application Security Testing)](#iast-interactive-application-security-testing)
    - [Kubernetes Tools](#kubernetes-tools)
    - [Infrastructure Tools](#infrastructure-tools)
- [Awesome Lists](#awesome-lists)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# Education

## Secure Development Processes

* [OWASP secure coding practices](https://www.owasp.org/images/0/08/OWASP_SCP_Quick_Reference_Guide_v2.pdf)
* [Go-SCP](https://checkmarx.gitbooks.io/go-scp/) - Golang specific secure coding practices

## Awareness of Security Risks

* [OWASP Top 10](https://www.owasp.org/images/7/72/OWASP_Top_10-2017_%28en%29.pdf.pdf) - Top 10 security risks from OWASP 2017

## Vulnerable Target Testing

* [Metasploitable](https://metasploit.help.rapid7.com/docs/metasploitable-2-exploitability-guide) - Vulnerable Linux image for testing
* [NodeGoat](https://github.com/owasp/nodegoat) - Vulnerable NodeJS app for testing
* [JuiceBox](https://www.owasp.org/index.php/OWASP_Juice_Shop_Project) - App for security testing education, includes the top 10 OWASP security risks

# Tools and Resources

## Application Testing Tools

### SAST (Static Application Security Testing)

SAST tools analyse source code to look for security issues in an application during non-running state, and are supported by a large number of languages. They usually have quite a high false positive rate, due to the fact they cannot track data through an app, instead using a bit of guesswork to determine if flaws exist.

* [Snyk](https://snyk.io/) - Dependency scanning, JS and Go
* [auditjs](https://www.npmjs.com/package/auditjs) - Dependency scanning, JS
* [clair](https://github.com/coreos/clair) - Container vulnerability scanning, Docker
* [Container Registry](https://cloud.google.com/container-registry/docs/get-image-vulnerabilities) - Container vulnerability scanning, Docker
* [Github Security Alerts](https://help.github.com/articles/about-security-alerts-for-vulnerable-dependencies/) - Dependency scanning, multiple languages
* [gosec](https://github.com/securego/gosec) - Golang
* [NodeJsScan](https://github.com/ajinabraham/NodeJsScan) - JS

### DAST (Dynamic Application Security Testing)

DAST tools run automated penetration testing scans against a running service as a blackbox. It tries to hack into the service using well known vulnerabilities, however scans can take a while due to the vast number, as well as crawling services to find all the endpoints.

* [OWASP ZAP](https://github.com/zaproxy/zaproxy)

### IAST (Interactive Application Security Testing)

IAST tools run security tests while the application is in use in production, working by using instrumentation. They have much lower false positive rates as they analyse real data running through the system, and provide immediate feedback.

* None we've tried yet

## Kubernetes Tools

* [Kubesec.io](https://kubesec.io/) - Quantifies risk for Kubernetes resources
* [Sysdig Falco](https://sysdig.com/opensource/falco/) - Container runtime security, alerts to potential security risks using defined rules

## Infrastructure Tools

* [OpenVAS](http://www.openvas.org/) - Vulnerability scanner of servers, internally and externally
* [Gauntlt](http://gauntlt.org/) - BDD-style vulnerability tester using multiple tools, good for regression testing
* [OWASP OWTF](https://www.owasp.org/index.php/OWASP_OWTF) - Penetration testing tool
* [Forseti Security](https://forsetisecurity.org/) - Google Cloud Platform specific security scanner
* [John the Ripper](https://www.openwall.com/john/) - Password cracking tool
* [Sysdig Inspect](https://sysdig.com/opensource/inspect/) - Capturing and analysis of kernel level instrumentation

## Other Tooling

* [Social Engineering Toolkit](https://github.com/trustedsec/social-engineer-toolkit)
* [Kali Linux](https://kali.org/) - SecOps Linux OS with multiple tools available for use

# Awesome Lists

* [Awesome DevSecOps](https://github.com/devsecops/awesome-devsecops)
* [Awesome Static Analysis](https://github.com/mre/awesome-static-analysis)
* [Awesome Kubernetes](https://github.com/ramitsurana/awesome-kubernetes)
