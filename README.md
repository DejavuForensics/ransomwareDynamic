# Repository
**Re**trieval of Ransomware **A**pplied to **D**ynamic **A**nalysis

## Limitation of Commercial Antivirus

Although it has been questioned for more than a decade, the modus operandi of antiviruses is based on signatures when the suspect file is consulted on datasets named blacklist. Therefore, it is enough that the hash of the investigated file not to be in the blacklist of the antivirus in order to malware not to be detected. The hash functions as a unique identifier for a given file. Then, given the limitations of commercial antiviruses, it is not a difficult task to develop and to distribute variants of a malicious application. To do this, it is enough to make small alterations in the original malware with routines that, effectively, do not have any usefulness like repetition loops and conditional branches without instructions in their scopes. These alterations without usefulness, however, they turn the hash of the modified malware different from the hash of the original malware. Consequently, malware, incremented with null routines, will not be detected by the antivirus which cataloged the original malware. It should to emphasize the existence of botnets responsible for creating and distributing, in automated form, variants of a same original malware. It is concluded that antiviruses, based on signatures, have null effectiveness when submitted to variants of a same malware.

Through the VirusTotal platform, this proposed paper investigates 77 commercial antiviruses with their respective results presented in Table 1. We used 998 ransomware malicious obtained from the base repository. The goal of the paper is to verify the amount of virtual plagues cataloged by antivirus. The motivation is that the acquisition of new virtual plagues plays an important role in combating malicious applications. Therefore, as larger is the dataset, named blacklist, better tends to be the defense provided by the antivirus. Fig. 1 shows the diagram of the methodology proposed in diagram of blocks. Initially, ransomware malwares are sent to the server belonging to the VirusTotal platform. After this, the ransomware Files are analyzed by the 86 commercial antiviruses from VirusTotal. Then, the antiviruses provide their diagnostics for ransomware files submitted to the server. VirusTotal allows the possibility of emission of three different types of diagnostics: malware, benign and omission.

As for the first possibility of VirusTotal, the antivirus detects the malignity of the suspicious file. In the proposed experimental environment, all submitted files are malware documented by incident responders. Then, the antivirus hits when it detects the malignity of the file investigated. Malware detection indicates that the antivirus provides a robust service against cyber-invasions. In the second possibility, the antivirus attests to the benignity of the investigated file. Therefore, in the proposed study, when the antivirus alleges the benignity of the file, it is a case of false negative because all submitted samples are malicious. That is, the file investigated is malware, however, the antivirus attests to benignity in a mistaken way. In the third possibility, the antivirus does not emit opinion about the suspect file. The omission indicates that the file investigated has never been evaluated by the antivirus so little it has the robustness to evaluate it in real time. The omission of the diagnosis by the antivirus points to its limitation on large-scale services.

Table 1 shows the results of the 86 antiviruses products evaluated. The McAfee-GW-Edition antivirus achieved the best performance by being able to detect 99.10% of the investigated malwares. A major adversity in order to combat malicious applications is the fact that the antivirus manufacturers do not share their malwares blacklists due to commercial disputes. Through the analysis of Table 1, the proposed work points to an aggravating factor of this adversity: the same antivirus manufacturer does not share their databases amongtheir different antiviruses. Observe, for example, that McAfee-GW-Edition and McAfee antiviruses belong to a same company. Their blacklists, though robust, are not shared amongst themselves. Therefore, the commercial strategies, of a same company, disturb the confrontation against malwares. It complements that antivirus manufacturers are not necessarily concerned in avoiding cyber-invasions, but in optimizing their business incomes.

Malware detection ranged from 0% to 99.10%, depending on the investigated antivirus. On average, the 86 antiviruses were able to detect 34.95% of the evaluated virtual plagues, with a standard deviation of 40.92. The high standard deviation indicates that the detection of malicious files can suffer abrupt variations depending on the chosen antivirus. It is determined that the protection, against cybernetic invasions, is in function of the choice of a robust antivirus with a large and updated blacklist. On average, antiviruses attested false negatives in 33.90% of the cases, with a standard deviation of 40.45. To attest the benignity of malware can implicate in unrecoverable damages. A person or institution, for instance, would start to trust on a certain malicious application when, in fact, it is a malware. Still as an unfavorable aspect, about 31.39% of antiviruses did not express an opinion on any of the 998 malicious samples. On average, the antiviruses were omitted in 31.15% of the cases, with a standard deviation of 45.61%. The omission of the diagnosis points to the limitation of antiviruses as for the malwares detection in real time.

It is included as adversity, in the combat to malicious applications, the fact of the commercial antiviruses do not have a pattern in classification of malwares as seen in Table 2. We chose 3 of the 998 ransomware malwares in order to exemplify the miscellaneous of classifications given by antivirus commercial activities. As there is no pattern, the antiviruses give the names that they want, for example, a company can identify a ransomware malware as "Android: RuFraud-I" and a second company identify it as "Artemis! 9EF6966B98A5". Therefore, the lack of a pattern disturbs the cyber-security strategies since each category of malware must have different treatments (vaccines). It is concluded that it is impracticable to a supervised machine learning adopts pattern recognition as for categories of ransomware malwares. Due to this confusing tangle of MultiClass Classification, provided by specialists (antiviruses) as seen in Table 4, it is statistically improbable that any machine learning technique will acquire generalization capability.

###### Table 1 – Results of 86 commercial antiviruses.

| Antivirus            | Detection (%) | False negative (%) | Omission (%) |
|----------------------|---------------|--------------------|--------------|
|Alibaba	             |99.45          |	0.55              |	0            |
MicroWorld-eScan	99,36	0,64	0
Webroot	99,36	0,36	0,27
FireEye	99,18	0,18	0,64
Fortinet	99,18	0,73	0,09
MAX	98,91	0,64	0,45
BitDefender	98,91	0,91	0,18
Panda	98,45	1,36	0,18
VIPRE	98,36	0,82	0,82
McAfee	98,27	0,45	1,27
Comodo	98,27	1,36	0,36
Microsoft	98,18	1	0,82
Emsisoft	98	0,91	1,09
GData	97,91	0,64	1,46
NANO-Antivirus	97,73	2,09	0,18
VBA32	97,54	2,27	0,18
Symantec	97,27	0,27	2,46
CrowdStrike	97,27	2,64	0,09
ESET-NOD32	97,18	2,73	0,09
Kaspersky	97,18	1,82	1
APEX	97,09	2,91	0
AVG	96,72	0,09	3,18
Jiangmin	96,54	3,28	0,18
Avast	96,09	2,37	1,55
SentinelOne	95,91	3,82	0,27
DrWeb	95,27	4,55	0,18
Rising	95,18	4,09	0,73
Tencent	94,72	4,91	0,36
TrendMicro-HouseCall	93,9	5,55	0,55
McAfee-GW-Edition	93,18	0,91	5,91
Sophos	93,18	1,73	5,1
ALYac	92,9	3,82	3,28
K7GW	92,63	7,37	0
K7AntiVirus	92,54	7,28	0,18
AhnLab-V3	92,54	7,46	0
TrendMicro	92,54	6,1	1,36
Cylance	92,45	3,82	3,73
Avira	92,45	7,46	0,09
Ad-Aware	91,63	3,91	4,46
Sangfor	91,63	2	6,37
Antiy-AVL	90,81	5,55	3,64
Zillya	90,72	6,28	3
Cynet	90,35	0,36	9,28
Elastic	85,99	4	10,01
Cyren	85,9	14,01	0,09
Yandex	85,44	14,56	0
Ikarus	85,26	7,01	7,73
Malwarebytes	84,53	15,1	0,36
Paloalto	82,98	16,92	0,09
Acronis	82,89	12,56	4,55
Lionic	77,62	19,38	3
Cybereason	74,16	0,36	25,48
BitDefenderTheta	72,25	24,39	3,37
MaxSecure	70,79	26,66	2,55
CAT-QuickHeal	70,52	29,21	0,27
SUPERAntiSpyware	66,61	33,39	0
ClamAV	66,61	30,03	3,37
Bkav	63,42	33,76	2,82
ZoneAlarm	55,32	40,22	4,46
VirIT	55,23	21,84	22,93
Kingsoft	55,14	43,86	1
ViRobot	49,04	50,96	0
Arcabit	45,77	49,77	4,46
TACHYON	43,31	56,69	0
Baidu	40,58	58,6	0,82
Gridinsoft	37,4	53,05	9,55
eGambit	30,03	14,83	55,14
F-Secure	10,56	89,08	0,36
Qihoo-360	9,83	11,37	78,8
Invincea	8,83	0,45	90,72
Endgame	7,46	0,55	91,99
F-Prot	6,19	1,73	92,08
Trapmine	5,28	2,09	92,63
Zoner	2,82	96,54	0,64
TotalDefense	1,36	7,1	91,54
CMC	1	98,73	0,27
Avast-Mobile	0	8,1	91,9

###### Table 2 – Miscellaneous classifications of commercial antiviruses.

| Antivirus            | VirusShare_A                                |           VirusShare_B                      | 
|----------------------|---------------------------------------------|---------------------------------------------|
McAfee-GW-Edition	 |	Artemis!Trojan	 |		PWS-Zbot.gen.jr |
NANO-Antivirus |	Trojan.Android.SMSSend.numyx  |		Trojan.Java.CVE20113544.cspflc |
AegisLab |	Troj.Sms.Androidos!c	  |	Troj.W32.Generic!c |
Kaspersky |	HEUR:Trojan-SMS.AndroidOS.Fakelogo.a |	HEUR:Trojan.Win32.Generic |
ZoneAlarm |	HEUR:Trojan-SMS.AndroidOS.Fakelogo.a |	HEUR:Trojan.Win32.Generic |
Avast |	Android:RuFraud-I	 |	Java:CVE-2011-3544-BD |
AVG |	Android:RuFraud-I	 |	Java:CVE-2011-3544-BD |
ESET-NOD32 |	Android/TrojanSMS.Agent.K  |	a variant of Java/Exploit.CVE-2011-3544.DF |
McAfee |	Artemis!9EF6966B98A5   |	RDN/Generic |
Avira |	ANDROID/SmsAgent.CQ.Gen  	 |	EXP/CVE-2011-3544 |
Sophos |	Andr/Jifake-B	 |	Mal/Generic-S|
Symantec |	Android.Fakemini	 	 |	Trojan.MalJava|
Ikarus |	Trojan.AndroidOS.FakeInst	  |	Java.CVE|
MAX |	Malware |	Malware |
TrendMicro-HouseCall |	Suspicious_GEN.F47V0322 |		Suspicious_GEN.F47V0322 |
Emsisoft |	Android.Trojan.FakeInst.CB |		Gen:Variant.Barys.841 |
GData |	Android.Trojan.FakeInst.CB	 |	Gen:Variant.Barys.84|
BitDefender |	Android.Trojan.FakeInst.CB	 |	Gen:Variant.Barys.84|
Tencent |	Trojan.Android.FakeLogo.aa	 |		Win32.Trojan.Jorik.Hvje|
Arcabit	 |	Android.Trojan.FakeInst.CB	 |		Trojan.Barys.841 |
MicroWorld-eScan |	Android.Trojan.FakeInst.CB	 |	Gen:Variant.Barys.84 |

## Materials and Methods

The present paper aims to elaborate the repository (Retrieval of ransomware Files Applied to Dynamic Analysis), a dataset which allows the classification of files with ransomware extension between benign and malwares. The repository is composed of 998 malware ransomware files and 998 other benign ransomware files. The repository dataset, consequently, is suitable for learning endowed with AI (Artificial Intelligence), considering that the ransomware files presented the same amount in the different classes (malware and benign). The goal is that tendentious classifiers, in relation to a certain class, do not have their success taxes favored.

In relation to virtual plagues, repository extracted malicious ransomware files from VirusShare which is a repository of malware samples to provide security researchers, incident responders, forensic analysts, and the morbidly curious access to samples of live malicious code. 
In order to catalog the 998 samples of ransomware malwares, it was necessary to acquire and analyze, by authorial script, about 3 million malwares from the reports updated by VirusShare daily. 
With respect to benign ransomware files, the catalog was given from application repositories such as Java2s.com, and findransomware.com. All of the benign files have been audited by VirusTotal. Then, the benign ransomware files, contained in repository, had their benevolence attested by the main commercial antiviruses of the world. The obtained results corresponding to the analyses of the benign and malware ransomware files, resulting from the VirusTotal audit, are available for consultation at the virtual address of repository.

The goal of creation of repository dataset is to give full possibility of the proposed methodology being replicated by third parties in future works. Then, repository makes available, freely, of all their samples such as benign as malwares:

• VirusTotal audits;

• Dynamic analysis of Cuckoo Sandbox.

repository also makes available in its virtual address, its 998 benign ransomware files. In addition, our dataset displays the list of all other 998 ransomware files, this time, malwares. Then, there is the possibility of the acquisition of all the malwares, employed by repository, through the agreement establishment and submission to the rules of use of ViruShare. It is concluded that our repository dataset enables transparency and impartiality to the research, in addition to demonstrating the veracity of the achieved results. Therefore, it is expected that repository serves as base for the creation of new scientific works aiming NGAVs.

## Dynamic Feature Extraction

The features of ransomware files originate through the dynamic analysis of suspicious files. Therefore, in our methodology, the malware is executed in order to infect, intentionally, the JVM installed in Windows 7 audited, in real time (dynamic), by the Cuckoo Sandbox. In total, 6,824 features are generated of each ransomware file, regarding the monitoring of the suspect file in the proposed controlled environment. Next, the groups of features are detailed.


###### Table 3 –  Descrição das características .

| Característica       | Descrição de parte das características      |       
|----------------------|---------------------------------------------|
signatures_"signatures"	|Uma breve descrição do que a assinatura representa. |
signatures_"ttp"	|Táticas, técnicas e procedimentos (TTPs) mais comuns de ataques cibernéticos |
signatures_"T1045"	|Uma tática de evasão de defesa, o T1045 está vinculado ao uso de tempo de execução ou empacotadores de software que ocultam arquivos desagradáveis, incluindo executáveis maliciosos|
signatures_"call"	|Chamadas de API|
signatures_"arguments"	|Argumentos referenciados das chamadas de API|
signatures_"T1082"	|Meios para coletar informações detalhadas sobre o status de segurança de um sistema operacional, hardware e software.|
signatures_"T1129"	|Carregador de módulo do Windows pode ser instruído a carregar DLLs de caminhos locais arbitrários e caminhos de rede arbitrários de convenção de nomenclatura universal (UNC). |Essa funcionalidade reside em NTDLL.dll e faz parte da API nativa do Windows que é chamada de funções como CreateProcess(), LoadLibrary(), etc. da API Win32.|
signatures_"T1057"	|Os adversários podem tentar obter informações sobre processos em execução em um sistema. As informações obtidas podem ser usadas para obter uma compreensão do software comum executado em sistemas dentro da rede|
signatures_"references"	|Lista de referências (URLs) para contextualizar a assinatura|
signatures_"ioc"	|Objeto ou atividade que, observado em uma rede ou em um dispositivo, indica uma alta probabilidade de acesso não autorizado ao sistema - em outras palavras, que o sistema está comprometido |
signatures_"T1012"	|Os adversários podem interagir com o Registro do Windows para coletar informações sobre o sistema, configuração e software instalado.|
signatures_"T1053"	|Utilitários como at e schtasks, juntamente com o Agendador de Tarefas do Windows, podem ser usados para agendar programas ou scripts a serem executados em uma data e hora. Uma tarefa também pode ser agendada em um sistema remoto, desde que a autenticação adequada seja atendida para usar RPC e o compartilhamento de arquivos e impressoras esteja ativado. Agendar uma tarefa em um sistema remoto normalmente exigia ser um membro do grupo Administradores no sistema remoto."|
signatures_"T1060"	|Adicionar uma entrada às \"chaves de execução\" no Registro ou pasta de inicialização fará com que o programa referenciado seja executado quando um usuário fizer login. Esses programas serão executados no contexto do usuário e terão o nível de permissões associado à conta."|
signatures_"families"	|uma lista de nomes de família de malware, caso a assinatura corresponda especificamente a um conhecido.|
signatures_"T1143"	|As configurações de como os aplicativos são executados no macOS e OS X são listadas nos arquivos de lista de propriedades (plist). Uma das tags nesses arquivos pode ser apple.awt.UIElement, que permite que aplicativos Java impeçam que o ícone do aplicativo apareça no Dock. Um uso comum para isso é quando os aplicativos são executados na bandeja do sistema, mas também não querem aparecer no Dock. No entanto, os adversários podem abusar desse recurso e ocultar sua janela de execução.|
signatures_"regkey"	|Indica a chave de registro acessada|
signatures_"regkey_r"	|Endereço da chave de registro|
signatures_"T1158"	|Arquivos e diretórios ocultos|
signatures_"T1106"	|Funções como a API do Windows CreateProcess permitirão que programas e scripts iniciem outros processos com parâmetros de caminho e argumento adequados."|
signatures_"c2"	|APIs de keylogging|
signatures_"c9"	|Conecta-se a hosts suspeitos|
signatures_"c7"	|Instalação no Autorun|
signatures_"c3"	|APIs de rede|
signatures_"c6"	|Porcentagem de pacotes de saída|
signatures_"c11"	|Acessa dados de bitcoin|
signatures_"c10"	|Deleta o binário original|
signatures_"c5"	|Número de arquivos acessados|
signatures_"category": |"pdb_path", 	Banco de dados de programas (PDB) é um formato de arquivo (desenvolvido pela Microsoft) para armazenar informações de depuração sobre um programa (ou, geralmente, módulos de programa, como DLL ou EXE). Os autores de malware na maior parte dos casos precisam depurar   seu código e utilizam o PDB para isso.|
signatures_"category": "file" 	|Descreve o tipo de evento relacionado a arquivo.|
signatures_"category": "process" 	|Descreve o tipo de evento relacionado ao processo executado.|
signatures_"category": "Jiangmin" 	|Descreve o tipo de evento relacionado ao resultado da identificação do antivirus Jiangmin.|
signatures_"category": "Antiy-AVL"	|Descreve o tipo de evento relacionado ao resultado da identificação do antivirus Antiy-AVL.|
signatures_"category": "Malwarebytes" |	Descreve o tipo de evento relacionado ao resultado da identificação do antivirus Malwarebytes.|



