#use sparingly - input many and miss info
>BPF syntax -expression has 1 or more primitives. Primitives have 1 or more qualifiers. the whole below is an expression, statement before an operator is a primitive, inside primitive is a qualifier and Ids(numbrs)
rfc 792(check. more technical)

icmp[0:2]==0x0301 2byte checking, destination unreachable host unreachable ->
(qualifier)(indexing operator)(relational operator)(numerical literal) ->
(primitives) (operator) (constant)

tcp[13] $8 ==8 flags are set in offset 13 each flag is identified by a bit. 32=urg, 16,ack, 8=psh, 4=rst, 2=syn, 1=fin
icmp - icmp traffic ONLY
ip - ipv4 ONLY | ip6 - ipv6 ONLY
broadcast - broadcast ONLY
ether host 00:00:00:00:00:00 - traffic to and from my mac address
