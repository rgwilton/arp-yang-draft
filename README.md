2019/02/25 updates
1.remove global-static-entries and arp-probe nodes in the arp model
2.update the description text of gratuitous-arp and add references of rfc related

-------------------------------------------

modification includes:
1.proxy arp extension 

2. 09/01/2018 Tom Petch

- YANG module copyright is 2016 which will get fixed but makes me notice ....

- Security Considerations is not the current template; should have Normative References to SSH and TLS

- s5.1 has
draft [I-D.ietf-netmod-rfc7277bis]).
which is now an RFC

- IANA Considerations references RFC7950.  As I learnt lately, RFC6020 is better here as all RFC7950 does is point you to RFC6020

-
"MAC address in the format of H-H-H, in which H is a  hexadecimal number of 1 to 4 bits.";

If H has a maximum of 4 bits, then you have a 12 bit address, not quite the MAC I see these days!  I wonder if it is better to leave this out and let readers refer to RFC6991.



version1 has addressed the following comments：
# arp-yang-draft
IETF draft for ARP YANG model

Comments of Tom Petch
1.08/02/2018
Another YANG I-D from the Routing Area; 

- Abstract contains a [Reference]

- No reference for YANG Tree Diagrams

- No mention of the current YANG 1.1 RFC

- No YANG version statement in the module

- No mention of NMDA in the body of the I-D (but it does appear in the YANG Module)

- No references for the imported modules and the RFC in question do not appear in the I-D Normative References

- YANG module references RFC8242 which does not appear in the I-D Normative References

- RFC 6536 is obsolete

2.07/31/2018
This I-D

- fails to mention whether or not it is NMDA compliant in the Abstract and Introduction

- fails to use the current definitions of terminology from RFC8342

- references the old version of RFC2119 key words

- has no Note to the RFC Editor asking them to replace the YANG module dates with date of publication.  I suggest a Note asking them to replace XXXX with the number assigned to this I-D at the start of the I-D rather than asking them to replace 'draft-ding-rtgwg-arp-yang-model-02 ' which, should this I-D be adopted, will be wrong

- has no Copyright statement in the YANG module

- lacks references for several imported modules.

- starts Section 4 well with a good sentence but fails to mention most imports

- has serious formatting problems with the text in the YANG module with lines being way too long for an RFC (it is probably not a coincidence that other I-Ds have had the same problem -  the right options in pyang fix this AFAIK)

- has no IANA Considerations; no IANA Considerations means that you are not producing a YANG module no matter what it looks like.

- Security Considerations are much better than usual but lack detail of sensitive nodes

- Tree diagrams has the right reference but then spoils it by including text about the symbols

- has out of date references
   [I-D.ietf-netmod-rfc7223bis]
   [I-D.ietf-netmod-rfc7277bis]
which belie the claimed date of  June 28, 2018 for this I-D; 2018-01-27 looks more like it:-)

- has arp as a Informative Reference - Normative I think.



