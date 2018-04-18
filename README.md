# libraries

A curated collection of cryptographic libraries. For each library, we provide a
a brief description of its main features.

- [libraries](#libraries)
    - [Python](#python)
        - [cryptography.io](#cryptographyio)
        - [Keyczar](#keyczar)
        - [M2Crypto](#m2crypto)
        - [pyNaCl](#pynacl)
        - [pyOpenSSL](#pyopenssl)
        - [PyCrypto](#pycrypto)
        - [PyCryptodome](#pycryptodome)
        - [pysodium](#pysodium)
    - [C](#c)
        - [OpenSSL](#openssl)
    - [Java](#java)
        - [Bouncy Castle](#bouncycastle)

------

## [Python](Python/)

#### cryptography.io

Python cryptographic interface built on top of the OpenSSL cryptographic library
(written in C). Provides high level recipes for authenticated encryption and
X.509 certificate management. Low level (hazmat) primitives provided for general
cryptographic operations.

- Developer: [Python Cryptographic Authority (PyCA)](https://github.com/orgs/pyca/people)
- Initial Release: 01/08/2014
- Latest version: 2.2.1 (03/20/2018)
- Languages: Python
- License: [Apache 2.0](http://apache.org/licenses/LICENSE-2.0) or
           [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)

[Website](https://cryptography.io/en/latest/) -
[GitHub](https://github.com/pyca/cryptography) -
[PyPi](https://pypi.python.org/pypi/cryptography/) -
[Documentation](https://cryptography.io/en/latest/)

#### Keyczar

High-level interface for a limited set of cryptographic operations and key
management built on top of lower-level libraries. Designed to provide safe and
easy access to cryptographic resources. All configuration is done through key
generation, which is accomplished through an included command-line tool.

- Developer: [Community Project](https://github.com/google/keyczar/wiki/Contributors)
- Initial Release: 12/28/2011
- Latest version: 0.716 (05/16/2016)
- Languages: Java, Python, C++
- License: [Apache 2.0](http://apache.org/licenses/LICENSE-2.0)

[Website](http://www.keyczar.org/) -
[GitHub](https://github.com/google/keyczar) -
[PyPi](https://pypi.python.org/pypi/python-keyczar) -
[Documentation](https://github.com/google/keyczar/wiki)

#### M2Crypto

Python interface built on top of the OpenSSL cryptographic library (written in
C). Provides access to a wide range of basic cryptographic operations as well
as SSL/TLS, HTTPS, S/MIME, X.509 Certificate management, etc. 

- Maintainer: [Matěj Cepl](https://matej.ceplovi.cz/)
- Initial Release: 06/24/2003
- Latest version: 0.29 (02/23/2018)
- Languages: Python
- License: [MIT](https://gitlab.com/m2crypto/m2crypto/blob/master/LICENCE)

[Website](https://gitlab.com/m2crypto/m2crypto) -
[GitLab](https://gitlab.com/m2crypto/m2crypto) -
[PyPi](https://pypi.python.org/pypi/M2Crypto) -
[Documentation](https://m2crypto.readthedocs.io/en/latest/)

#### PyCrypto 

Python library of cryptographic algorithms implemented in C.
Includes cryptographic algorithms for shared key and public key 
encryption and authentication, cryptographic hashes, and key derivation. 
Also provides a secure PRNG, a strong version of Python's random
module, and a small set of useful mathematical operations.

- Developer: [Dwayne Litzenberger](https://www.dlitz.net/)
- Initial Release: 11/11/2002
- Latest version: 2.6.1 (10/14/2013).
- Languages: Python
- License: [Public Domain (mostly, see license)](https://github.com/dlitz/pycrypto/blob/master/COPYRIGHT)

[Website](https://www.dlitz.net/software/pycrypto/) -
[GitHub](https://github.com/dlitz/pycrypto) -
[PyPi](https://pypi.python.org/pypi/pycrypto/2.6.1) -
[API documentation](https://www.dlitz.net/software/pycrypto/api/current/) -
[Configuration details](Python/PyCrypto.config)

#### PyCryptodome

Python library of cryptographic algorithms, partially implemented in C. Began as
a fork of PyCrypto. Continued development has added support for authenticated
encryption, safe stream ciphers, elliptic curve operations (encryption and
signing), SHA3 hash functions, etc.

- Developer: [Helder Eijs (Legrandin)](https://github.com/Legrandin)
- Initial Release: 6/24/2014
- Latest version: 3.5.1 (03/07/2018)
- Languages: Python
- License: [Public Domain, BSD-2-Clause](https://github.com/Legrandin/pycryptodome/blob/master/LICENSE.rst)

[Website](https://www.pycryptodome.org/en/latest/) -
[GitHub](https://github.com/Legrandin/pycryptodome) -
[PyPi](https://pypi.python.org/pypi/pycryptodomex) -
[Documentation](https://pycryptodome.readthedocs.io/en/latest/) -
[Configuration details](Python/PyCryptodome.config)

#### pyNaCl

A Python interface for the libsodium cryptographic library (written in C), a
fork of the Networking and Cryptography Library (NaCl). Libsodium (and NaCl) are
designed to provide easy access to a carefully selected set of cryptographic
algorithms implemented for saftey and efficiency. The pyNaCl interface provides
similarly high-level access to those resources from within the Python language.

- Developer: [Python Cryptographic Authority (PyCA)](https://github.com/orgs/pyca/people)
- Initial Release: 04/14/2013
- Latest version: 1.2.1 (12/04/2018)
- Languages: Python
- License: [Apache 2.0](https://github.com/pyca/pynacl/blob/master/LICENSE)

[Website](https://pynacl.readthedocs.io/en/stable/) -
[GitHub](https://github.com/pyca/pynacl) -
[PyPi](https://pypi.python.org/pypi/PyNaCl/) -
[Documentation](https://pynacl.readthedocs.io/en/stable/)

#### pyOpenSSL

A lightweight Python interface for a subset of the OpenSSL cryptographic
library (written in C). Does not provide general access to basic cryptographic
operations, but instead focuses on the construction of SSL/TLS sessions and the
lower-level cryptographic operations required to manage them (public key 
authentication and X.509 certificate handling).

- Developer: [Python Cryptographic Authority (PyCA)](https://github.com/orgs/pyca/people)
- Initial Release: 07/16/2001
- Latest version: 17.5.0 (11/30/2017)
- Languages: Python
- License: [Apache 2.0](https://github.com/pyca/pyopenssl/blob/master/LICENSE)

[Website](https://pyopenssl.org/en/stable/) -
[GitHub](https://github.com/pyca/pyopenssl) -
[PyPi](https://pypi.python.org/pypi/pyOpenSSL) -
[Documentation](https://pyopenssl.org/en/stable/)

#### pysodium

A lightweight interface wrapped around the libsodium cryptographic library
(written in C), a fork of the Networking and Cryptography library (NaCl). This
is practically a repoduction of the lower-level NaCl interface for cryptographic
operations slightly adapted for usage in Python.

- Developer: [Stefan Marsiske](https://www.ctrlc.hu/~stef/blog/)
- Initial Release: 08/25/2013
- Latest version: 0.7.0 (02/02/2018)
- Languages: Python
- License: [BSD-2-Clause](https://github.com/stef/pysodium/blob/master/pysodium/__init__.py)

[Website](https://github.com/stef/pysodium) -
[GitHub](https://github.com/stef/pysodium) -
[PyPi](https://pypi.python.org/pypi/pysodium)

------

## C

#### OpenSSL

------

## Java

#### Bouncy Castle

------

## Uncategorized

#### NTRU

- Languages: C, Java

[Website](https://www.onboardsecurity.com/products/ntru-crypto) -
[GitHub](https://github.com/NTRUOpenSourceProject/ntru-crypto)

------

# Other resources

- [Comparison of cryptography libraries](https://en.wikipedia.org/wiki/Comparison_of_cryptography_libraries)
- [Source available cryptographic libraries](https://adam.shostack.org/crypto/index.html)
- [Cryptographic software](https://en.wikipedia.org/wiki/Category:Cryptographic_software)
