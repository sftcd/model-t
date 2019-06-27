
# Notes for 20190627 call

As usual, just some notes for us to chat over.

Two thoughts for the day...

## A modest extension of 3552

3552 says:

            In general, we assume that the end-systems engaging in a protocol
            exchange have not themselves been compromised.

How about if, instead, that said:

            In general, we assume that one of the end-systems engaging in a
            protocol exchange has not been compromised.

V. small change in words, maybe enough to be interesting though?

## "not closed" I-D

At the IAB retreat we discussed someone writing a short I-D 
that says "that network you think is closed - it's not" or
some such. A possible outline for that might be:

- state the proposition
    - n/w forumulation: if you design a n/w assuming it's not connected to the Internet
    chances are, you'll end up wrong, so you should design it 
    assuming it will be connected to the Internet
    - protocol formulation: if you design a n/w protocol assuming its endpoints won't
    be connected to the Internet chances are, you'll end up wrong, so you should design it 
    assuming endopints will be connected to the Internet
    - system formulation: if you design a system assuming its components won't
    be connected to the Internet chances are, you'll end up wrong, so you should design it 
    assuming components will be connected to the Internet
- provide examples of when that assumption didn't pan out:
    - need to find examples with good refs to keep text short
    - stuxnet
    - some DB exposed to Internet incident
    - MPLS maybe
    - leaky home n/w devices
- what to do?
    - assume any n/w, protocol, system will be exposed to the
    Internet at some point
    
