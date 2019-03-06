# supress_list-snort-maral
supress_list snort

#(http_inspect) DOUBLE DECODING ATTACK
suppress gen_id 119, sig_id 2

#(http_inspect) U ENCODING
suppress gen_id 119, sig_id 3

#(http_inspect) NO CONTENT-LENGTH OR TRANSFER-ENCODING IN HTTP RESPONSE
suppress gen_id 120, sig_id 3

#(http_inspect) TOO MANY PIPELINED REQUESTS
suppress gen_id 119, sig_id 34

#(http_inspect) SIMPLE REQUEST
suppress gen_id 119, sig_id 32

#(http_inspect) INVALID CONTENT-LENGTH OR CHUNK SIZE
suppress gen_id 120, sig_id 8

#PROTOCOL-DNS potential dns cache poisoning attempt - mismatched txid
suppress gen_id 3, sig_id 21355

#PROTOCOL-DNS TMG Firewall Client long host entry exploit attempt
suppress gen_id 3, sig_id 19187

#(http_inspect) BARE BYTE UNICODE ENCODING
suppress gen_id 119, sig_id 4

#(http_inspect) IIS UNICODE CODEPOINT ENCODING
suppress gen_id 119, sig_id 7

#(http_inspect) UNESCAPED SPACE IN HTTP URI
suppress gen_id 119, sig_id 33

#ET INFO Session Traversal Utilities for NAT (STUN Binding Request)
suppress gen_id 1, sig_id 2016149

#(http_inspect) UNKNOWN METHOD
suppress gen_id 119, sig_id 31

#ET POLICY Outgoing Basic Auth Base64 HTTP Password detected unencrypted
suppress gen_id 1, sig_id 2006380

#(IMAP) Unknown IMAP4 command
suppress gen_id 141, sig_id 1

#ET DNS DNS Lookup for localhost.DOMAIN.TLD
suppress gen_id 1, sig_id 2011802

