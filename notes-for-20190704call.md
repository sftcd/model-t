
# More reading than writing this time...

I've been looking at bit at [rfc6819](https://tools.ietf.org/html/rfc6819),
the OAuth threat model. I've not finished re-reading it.

Some take-aways:

- it's too complicated to keep in my little head to be useful as
  design guidance, but maybe some abstract model for 3-legged
  protocols based on it could be 
- it covers more than 3552, for example one of their "attack
  assumptions" is:

              two of the three parties involved in the OAuth protocol may
              collude to mount an attack against the 3rd party.  For example,
              the client and authorization server may be under control of an
              attacker and collude to trick a user to gain access to resources.

  which sounds quite like what we've been thinking
- they also do consider locally stored configs/keys/trust anchors as things
  that are at-risk
- some of the concepts, e.g. bearer-token, do generalise nicely but it's
  not clear how much of it would - could be a bunch of work to figure
  that out - might be a useful exercise to find a protocol that's as
  "far" from OAuth as possible and see what maps well
- OAuth, given it's nature, does consider deployment as a specifically
  different thing from implementation.
- The big catalog of attacks in the RFC probably has lots of lessons,
  but I wonder how comprehensible it's been even for OAuth implementers,
  but we could ask!

Jari has started to write about closed networks
- See Section 4.2 in https://arkko.com/ietf/iab/draft-arkko-arch-internet-threat-model.diff.html
