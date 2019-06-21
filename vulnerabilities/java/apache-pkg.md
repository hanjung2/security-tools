# Apache Commons Collections
### Found in ver 2.9.1
Apache Commons Collections has a security flaw in the `InvokeTransformer` class whereby serializable collections can be built that execute arbitrary Java code. An attacker can achieve remote code execution (*RCE*) when untrusted user-provided objects are deserialized by applications that use Commons Collections.


The apache commons collection (ACC) library, when utilized in an application that deserializes untrusted user input, is vulnerable to a remote attacker executing arbitrary code.


Apache Common Collections and Apache Synapse contain a vulnerability that allows for remote code execution via crafted specialized objects. Failed attempts will cause a denial of service (*DoS*) attack.

# Apache Xerces
### Found in ver 2.9.1
Apache Xerces2 Java Parser before 2.12.0 allows remote attackers to cause a denial of service (CPU consumption) via a crafted message to an XML service, which triggers hash table collisions.


A remote attacker can supply a specially crafted XML file to an application linked to the Apache Xerces XML library that will cause excessive resource consumption resulting in a denial-of-service (*DoS*).


A flaw within XMLScanner.java of Xerces2-J allows remote attackers to perform a Denial of Service by causing an infinite loop condition via malformed XML. A number of sources incorrectly referenced CVE-2009-2625 when discussing other XML based vulnerabilities, including project expat *(http://seclists.org/oss-sec/2009/q4/67)*. A separate identifier was created for expat as: CVE-2009-3720. The fix for this vulnerability *(CVE-2009-2625)* is specific to xerces2_java. The entry provided by NVD specifically associates this identifier with both JDK and JRE. However, the vulnerability exists within the apache component Xerces2 Java which is widely used as a third party component.