# Cisco-Packet-Tracer
PIM III Unip Arujá

Classe de rede A:
	
R1 10.0.0.1/30 (255.255.255.252)	
R2 10.0.0.2/30 (255.255.255.252)
	
A Máscara foi escolhida para ter um menor desperdício de IP. Para conectar à rede precisa de 2 IP, (2^) - 2.
(24) = 4(-2) = 2 IP validos.

10.	0.	0.	1.
00001010.	00000000.	00000000.	00000001.
			                        0000|0001.
8.	8.	8.	4 .
255.	255.	255.	252

8 + 8 + 8 + 4 = 30 Máscaras.
Com isso conseguimos um menor desperdício de IP.

Classe de rede C:
 
	2SHOW.IE 192.168.2.1/25
	Sucursal 192.168.3.1/26

2SHOW.IE usa 64 hosts a máscara de rede é 25, (128 IP), a empresa contem 64 IP, por isso a máscara 26 (64) não poderia ser utilizada já que ela tem 62 IP validos (26) -2 = 62. O mais próximo, e a máscara 25, com 126 IP validos, (27) -2=126.

192.	168.	2.	1.
11000000.	10101000.	00000010.	00000001.
			                        0|0000000.
8.	8.	8.	1.
255.	255.	255.	128

	8 + 8 + 8 + 1 = 25 Máscaras.

Sucursal usa 32 hosts, a máscara de rede é 26, (64 IP) a máscara mais próxima é de 26 (64 IP) a máscara 27 (32 IP), não poderia ser utilizada porque só tem 30 IP validos, (25) -2 =30. 
A 26 (26) -2 = 62 IP validos. 

192.	168.	3.	1.
11000000.	10101000.	00000011.	00000001.
			                        00|000000.
8.	8.	8.	2.
255.	255.	225.	192
	
	8 + 8 + 8 + 2 = 26 Máscaras.


