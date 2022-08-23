# Ransomware
Analise de Malwares Ransomware via Redes Neurais

## Limitações dos Antivirus Comerciais

Tecnicamente, o modus operandi para a identificação de arquivos e servidores maliciosos refere-se à consulta em bases de dados de listas negras nomeadas. A plataforma VirusTotal emite os diagnósticos de características malignas relacionadas a arquivos e servidores web.

Quando se trata de arquivos suspeitos, o VirusTotal emite os diagnósticos fornecidos pelos principais produtos antivírus comerciais do mundo. Em relação aos servidores web suspeitos, o VirusTotal utiliza o banco de dados responsável por detectar endereços virtuais com práticas maliciosas.

O VirusTotal possui Application Programming Interface (APIs) que permitem aos programadores consultar a plataforma de forma automatizada e sem o uso da interface gráfica da web. O artigo proposto emprega duas das APIs disponibilizadas pelo VirusTotal. O primeiro é responsável por enviar os arquivos investigados ao servidor da plataforma. A segunda API, por sua vez, disponibiliza diagnósticos antivírus comerciais para arquivos enviados à plataforma pela primeira API.

Inicialmente, os malwares executáveis ​​são enviados ao servidor pertencente à plataforma VirusTotal. Depois disso, os executáveis ​​são analisados ​​pelos 86 antivírus comerciais vinculados ao VirusTotal. Portanto, o antivírus fornece seu diagnóstico para os executáveis ​​submetidos à plataforma. O VirusTotal permite a emissão de três tipos diferentes de diagnósticos: malware, benigno e omissão.

Em seguida, através da plataforma VirusTotal, o trabalho proposto investiga 68 antivírus comerciais com seus respectivos resultados apresentados na Tabela 2. Utilizamos 1000 executáveis ​​maliciosos para ARM obtidos de nosso banco de dados. O objetivo do trabalho é verificar o número de pragas virtuais catalogadas por antivírus. A motivação é que a aquisição de novas pragas virtuais desempenha um papel importante no combate a aplicativos maliciosos. Portanto, quanto maior o banco de dados de malwares na lista negra, melhor tende a ser a defesa fornecida pelo antivírus.

Quanto à primeira possibilidade do VirusTotal, o antivírus detecta a malignidade do arquivo suspeito. No ambiente experimental proposto, todos os executáveis ​​enviados são malwares de domínio público. Portanto, no estudo proposto, o antivírus acerta quando detecta a malignidade do executável investigado. A detecção de malware indica que o antivírus fornece um serviço robusto contra invasões cibernéticas. Quanto maior o banco de dados da lista negra, melhor tende a ser a defesa fornecida pelo antivírus.

Na segunda possibilidade, o antivírus atesta a benignidade do arquivo investigado. Portanto, no estudo proposto, quando o antivírus atesta a benignidade do arquivo, trata-se de um falso negativo – já que todas as amostras são maliciosas. Ou seja, o executável investigado é um malware; no entanto, o antivírus atesta a benignidade da maneira errada.

Na terceira possibilidade, o antivírus não emite opinião sobre o executável suspeito. A omissão indica que o arquivo investigado nunca foi avaliado pelo antivírus nem tem robustez para avaliá-lo em tempo real. A omissão do diagnóstico pelo antivírus aponta para sua limitação em serviços de grande porte.

Na terceira possibilidade, o antivírus não emite opinião sobre o executável suspeito. A omissão indica que o arquivo investigado nunca foi avaliado pelo antivírus nem tem robustez para avaliá-lo em tempo real. A omissão do diagnóstico pelo antivírus aponta para sua limitação em serviços de grande porte.

A Tabela 2 mostra os resultados dos 68 produtos antivírus avaliados. Apenas um desses antivírus obteve pontuação acima de 82,6%. Este antivírus é: ESET-NOD32. A detecção de malware indica que esses programas antivírus fornecem um serviço eficiente contra invasões cibernéticas.

Uma grande adversidade no combate a aplicativos maliciosos é o fato de os fabricantes de antivírus não compartilharem suas listas negras de malware devido a disputas comerciais. Por meio da análise da Tabela 2, o trabalho proposto aponta para um agravante dessa adversidade: o mesmo fornecedor de antivírus nem sequer compartilha seus bancos de dados entre seus diferentes programas antivírus. Observe, por exemplo, que os antivírus McAfee e McAfee-GW-Edition pertencem à mesma empresa. Suas listas negras, embora robustas, não são compartilhadas entre si. Portanto, as estratégias comerciais da mesma empresa dificultam o confronto com malware. Complementa que os fornecedores de antivírus não estão necessariamente preocupados em evitar invasões cibernéticas, mas em otimizar sua receita comercial.

A detecção de malware variou de 0% a 82,6%, dependendo do antivírus que está sendo investigado. Em média, os 68 antivírus foram capazes de detectar 46,08% das pragas virtuais avaliadas, com desvio padrão de 35,61. O alto desvio padrão indica que a detecção de executáveis ​​maliciosos pode sofrer variações abruptas dependendo do antivírus escolhido. Fica determinado que a proteção, contra invasões cibernéticas, se deve à escolha de um antivírus robusto com uma lista negra grande e atualizada.

Quanto aos falsos negativos, os antivírus Malwarebytes, Baidu e Panda, afirmaram erroneamente que o malware era benigno em mais de 95% dos casos. Em média, os antivírus atestaram falsos negativos em 44,85% dos casos, com desvio padrão de 36,26. Lidar com a benignidade do malware pode levar a danos irrecuperáveis. Uma pessoa ou instituição, por exemplo, confiaria em um determinado aplicativo malicioso quando, na verdade, é um malware.

As empresas de antivírus Invincea, CrowdStrike, eGambit e F-Prot dificilmente retiveram opiniões sobre qualquer uma das 1.000 amostras maliciosas. Portanto, cerca de 7,35% dos softwares antivírus não foram capazes de diagnosticar um número mínimo significativo de amostras maliciosas. Em média, os antivírus estavam ausentes em 8,92% dos casos, com desvio padrão de 25,76. A omissão do diagnóstico aponta para a limitação desses antivírus que possuem listas negras limitadas para detecção de malware em tempo real.

Inclui-se como adversidade, no combate às aplicações maliciosas, o fato dos antivírus comerciais não possuírem um padrão na classificação dos malwares como visto na Tabela 3. Escolhemos 3 de 1.000 amostras de malwares para exemplificar as classificações diversas de antivírus comerciais. Os malwares escolhidos são VirusShare_001627d61a1bde3478ca4965e738dc1e, VirusShare_075efef8c9ca2f675be296d5f56406fa e VirusShare_0dab86f850fd3dafc98d0f2b401377d5. Dessa forma, o tempo em que os fabricantes reagem a uma nova praga virtual é afetado drasticamente. Como não há um padrão, os antivírus dão os nomes que quiserem, por exemplo, uma empresa pode identificar um malware como "Trojan.Linux.Generic.69575" e uma segunda empresa o identifica como "ELF:DDoS-S [Trj] ". Portanto, a falta de um padrão, além do não compartilhamento de informações entre os fabricantes de antivírus, dificulta a detecção rápida e eficaz de um aplicativo malicioso.

###### Table 1 Results of 77 commercial antiviruses:

Antivirus |	Deteccion (%) |	False Negative (%) |	Omission (%)
--------- | ------------- | ------------------ | -------------
Alibaba |	99,45|	0,55|	0|
MicroWorld-eScan	|99,36|	0,64|	0|
Webroot	|99,36|	0,36|	0,27|
FireEye	|99,18|	0,18|	0,64|
Fortinet|	99,18|	0,73|	0,09|
MAX|	98,91|	0,64|	0,45|
BitDefender|	98,91|	0,91|	0,18|
Panda	98,45|	1,36|	0,18|
VIPRE|	98,36|	0,82|	0,82|
McAfee|	98,27|	0,45|	1,27|
Comodo|	98,27|	1,36|	0,36|
Microsoft|	98,18|	1|	0,82|
Emsisoft|	98|	0,91|	1,09|
GData|	97,91|	0,64|	1,46|
NANO-Antivirus|	97,73|	2,09|	0,18|
VBA32|	97,54|	2,27|	0,18|
Symantec	|97,27|	0,27|	2,46|
CrowdStrike	|97,27|	2,64|	0,09|
ESET-NOD32	|97,18|	2,73|	0,09|
Kaspersky	|97,18|	1,82|	1|
APEX|	97,09|	2,91|	0|
AVG|	96,72|	0,09|	3,18|
Jiangmin|	96,54|	3,28|	0,18|
Avast|	96,09|	2,37|	1,55|
SentinelOne|	95,91|	3,82|	0,27|
DrWeb|	95,27|	4,55|	0,18|
Rising|	95,18|	4,09|	0,73|
Tencent|	94,72|	4,91|	0,36|
TrendMicro-HouseCall|	93,9|	5,55|	0,55|
McAfee-GW-Edition	|93,18|	0,91|	5,91|
Sophos	|93,18|	1,73|	5,1|
ALYac	|92,9|	3,82|	3,28|
K7GW	92,63|	7,37|	0|
K7AntiVirus|	92,54|	7,28|	0,18|
AhnLab-V3|	92,54|	7,46|	0|
TrendMicro|	92,54|	6,1|	1,36|
Cylance	92,45|	3,82|	3,73|
Avira|	92,45|	7,46|	0,09|
Ad-Aware|	91,63|	3,91|	4,46|
Sangfor	|91,63|	2|	6,37|
Antiy-AVL|	90,81|	5,55|	3,64|
Zillya	|90,72	|6,28|	3|
Cynet	|90,35|	0,36|	9,28|
Elastic	|85,99|	4|	10,01|
Cyren	|85,9|	14,01|	0,09|
Yandex	|85,44	|14,56|	0|
Ikarus	|85,26|	7,01|	7,73|
Malwarebytes|	84,53|	15,1|	0,36|
Paloalto|	82,98|	16,92|	0,09|
Acronis|	82,89|	12,56|	4,55|
Lionic|	77,62|	19,38|	3|
Cybereason|	74,16|	0,36|	25,48|
BitDefenderTheta|	72,25|	24,39|	3,37|
MaxSecure|	70,79|	26,66|	2,55|
CAT-QuickHeal|	70,52|	29,21|	0,27|
SUPERAntiSpyware|	66,61|	33,39|	0|
ClamAV|	66,61|	30,03|	3,37|
Bkav|	63,42|	33,76|	2,82|
ZoneAlarm|	55,32|	40,22|	4,46|
VirIT|	55,23|	21,84|	22,93|
Kingsoft|	55,14|	43,86|	1|
ViRobot|	49,04|	50,96|	0|
Arcabit|	45,77|	49,77|	4,46|
TACHYON|	43,31|	56,69|	0|
Baidu|	40,58|	58,6|	0,82|
Gridinsoft|	37,4|	53,05|	9,55|
eGambit	30,03|	14,83|	55,14|
F-Secure|	10,56|	89,08|	0,36|
Qihoo-360|	9,83|	11,37|	78,8|
Invincea|	8,83|	0,45|	90,72|
Endgame|	7,46|	0,55|	91,99|
F-Prot|	6,19	1,73|	92,08|
Trapmine|	5,28|	2,09|	92,63|
Zoner	|2,82|	96,54|	0,64|
TotalDefense	|1,36|	7,1|	91,54|
CMC	|1	|98,73|	|0,27|
Avast-Mobile	|0	|8,1	|91,9|

###### Table 2 Miscellaneous classifications of commercial antiviruses:

Antivírus |	VirusShare_001627d61a1bde3478ca4965e738dc1e |	VirusShare_075efef8c9ca2f675be296d5f56406fa |	VirusShare_0dab86f850fd3dafc98d0f2b401377d5
--------- | ------------------------------------------- | ------------------------------------------- | --------------------------------------------
ALYac|Trojan.Linux.Generic.69575|Gen:Variant.Backdoor.Linux.Tsunami.1|Trojan.Linux.GenericA.73451|
AVG|ELF:DDoS-S [Trj]|ELF:Gafgyt-DO [Trj]|ELF:DDoS-S [Trj]|
Acronis|Undetected|Undetected|Undetected| 
Ad-Aware|Trojan.Linux.Generic.69575|Gen:Variant.Backdoor.Linux.Tsunami.1|Trojan.Linux.GenericA.73451|
AhnLab-V3|Linux/Mirai.Gen6|Linux/Tsunami.Gen|Linux/Gafgyt.Gen|
Antiy-AVL|Trojan[Backdoor]/Linux.Gafgyt.a|GrayWare/Linux.Generic|Trojan[Backdoor]/Linux.Gafgyt.ac|
Arcabit|Trojan.Linux.Generic.D10FC7|Trojan.Backdoor.Linux.Tsunami.1|Trojan.Linux.GenericA.D11EEB|
Avast|ELF:DDoS-S [Trj]|ELF:Gafgyt-DO [Trj]|ELF:DDoS-S [Trj]|
Avast-Mobile|ELF:DDoS-S [Trj]|ELF:Tsunami-CR [Trj]|ELF:DDoS-S [Trj]|
Avira|LINUX/Gafgyt.opnd|LINUX/Tsunami.wkuvt|LINUX/Gafgyt.opnd|
Baidu|Undetected|Undetected|Undetected| 
BitDefender|Trojan.Linux.Generic.69575|Gen:Variant.Backdoor.Linux.Tsunami.1|Trojan.Linux.GenericA.73451|
BitDefenderTheta|Gen:NN.Mirai.34608|Gen:NN.Mirai.34608|Gen:NN.Mirai.34608|
Bkav|Undetected|Undetected|Undetected| 
CAT-QuickHeal|Undetected|Elf.Trojan.A1198970|Undetected| 
CMC|Undetected|Undetected|Undetected| 
ClamAV|Unix.Malware.Agent-6769357-0|Unix.Trojan.Mirai-5607483-0|Unix.Trojan.Gafgyt-111|
Comodo|Malware@#3o8smwc385jui|Malware@#3j0a9lm761bhc|Malware@#1vbephabp2pmb|
Cynet|Malicious (score: 85)|Malicious (score: 85)|Malicious (score: 85)|
Cyren|E32/Gafgyt.C.gen!Camelot|E32/Gafgyt.C.gen!Camelot|E32/Gafgyt.C.gen!Camelot|
DrWeb|Linux.BackDoor.Fgt.1755|Linux.BackDoor.Tsunami.485|Linux.BackDoor.Fgt.9|
ESET-NOD32|a variant of Linux/Mirai.AE|a variant of Linux/Tsunami.NBV|a variant of Linux/Gafgyt.C|
Emsisoft|Trojan.Linux.Generic.69575 (B)|Gen:Variant.Backdoor.Linux.Tsunami.1 (B)|Trojan.Linux.GenericA.73451 (B)
F-Secure|Malware.LINUX/Gafgyt.opnd|Malware.LINUX/Tsunami.wkuvt|Malware.LINUX/Gafgyt.opnd|
FireEye|Trojan.Linux.Generic.69575|Gen:Variant.Backdoor.Linux.Tsunami.1|Trojan.Linux.GenericA.73451|
Fortinet|ELF/Mirai.AE!tr|ELF/Tsunami.NDJ!tr|ELF/Gafgyt.UN!tr.bdr|
GData|Linux.Trojan.Gafgyt.A|Linux.Trojan.Gafgyt.A|Linux.Trojan.Gafgyt.B|
Gridinsoft|Undetected|Undetected|Undetected| 
Ikarus|Trojan.Linux.Mirai|Trojan.Linux.Fgt|Trojan.Linux.Fgt|
Jiangmin|Backdoor.Linux.cbip|Backdoor.Linux.ksj|Backdoor.Linux.gmy|
K7AntiVirus|Undetected|Undetected|Undetected| 
K7GW|Undetected|Undetected|Undetected| 
Kaspersky|HEUR:Backdoor.Linux.Gafgyt.a|HEUR:Backdoor.Linux.Tsunami.bh|HEUR:Backdoor.Linux.Gafgyt.ac|
Kingsoft|Undetected|Undetected|Undetected| 
Lionic|Trojan.Linux.Gafgyt.4!c|malware (ai score=99)|Undetected| 
MAX|malware (ai score=99)|Undetected|malware (ai score=98)
Malwarebytes|Undetected|Trojan.Malware.121218.susgen|Undetected| 
MaxSecure|Trojan.Malware.121218.susgen|Linux/Gafgyt.h|Trojan.Malware.121218.susgen|
McAfee|Linux/Mirai.g|Linux/Gafgyt.h|Linux/Gafgyt.r|
McAfee-GW-Edition|Linux/Mirai.g|Gen:Variant.Backdoor.Linux.Tsunami.1|Linux/Gafgyt.r|
MicroWorld-eScan|Trojan.Linux.Generic.69575|Backdoor:Linux/Gafgyt.AF!MTB|Trojan.Linux.GenericA.73451|
Microsoft|DDoS:Linux/Gafgyt.YA!MTB|Trojan.ElfArm32.Tsunami.ejtrus|Backdoor:Linux/Gafgyt.AF!MTB|
NANO-Antivirus|Trojan.ElfArm32.Mirai.fkvjsm|Undetected|Trojan.ElfArm32.Gafgyt.emzwvw|
Panda|Undetected|Linux/Backdoor.9d5|Undetected| 
Qihoo-360|Linux/Backdoor.812|Trojan.Gafgyt/Linux!1.A480 (CLASSIC)|Linux/Trojan.DDoS.adc|
Rising|Backdoor.Mirai/Linux!1.BAF6 (CLASSIC)|Undetected|Backdoor.Gafgyt/Linux!1.A512 (CLASSIC)|
SUPERAntiSpyware|Undetected|Undetected|Undetected| 
Sangfor|Undetected|Linux/Tsunami-A|Malware.ELF-Script.Save.07a8c2d7|
Sophos|Linux/DDoS-CIA|Trojan.Gen.NPE|Linux/DDoS-BI|
Symantec|Trojan.Gen.NPE|Undetected|Linux.Lightaidra|
TACHYON|Undetected|Backdoor.Linux.Gafgyt.ya|Undetected| 
Tencent|Backdoor.Linux.Gafgyt.ff|Undetected|Backdoor.Linux.Gafgyt.ym|
TotalDefense|Undetected|Backdoor.Linux.BASHLITE.SMJC|Undetected| 
TrendMicro|Backdoor.Linux.BASHLITE.SMJC|Backdoor.Linux.BASHLITE.SMJC|Backdoor.Linux.BASHLITE.SMJC|
TrendMicro-HouseCall|Backdoor.Linux.BASHLITE.SMJC|Undetected|Backdoor.Linux.BASHLITE.SMJC|
VBA32|Undetected|Undetected|Undetected| 
VIPRE|Undetected|Undetected|Undetected| 
ViRobot|Undetected|Undetected|Undetected| 
Yandex|Undetected|Backdoor.Tsunami.Linux.379|Undetected| 
Zillya|Backdoor.Mirai.Linux.38039|HEUR:Backdoor.Linux.Tsunami.bh|Undetected| 
ZoneAlarm|HEUR:Backdoor.Linux.Gafgyt.a|Undetected|HEUR:Backdoor.Linux.Gafgyt.ac|
Zoner|Undetected|Undetected|Undetected| 

