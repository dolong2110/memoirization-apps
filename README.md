# Memorization App


## Application Overview

A chart of the tools and applications used is given below.

![App Overview](pictures/application_overview.png)

## Use Makefile to generate rsa256 keys

````
make create-keypair ENV=test
````

## Using Docker

each time change the code we should re-initialize the docker again at the root.

````
docker-compose up
````

can run a container that does not depend on other

````
docker-compose up postgres-account
````

## Migrate DB

````
make migrate-create NAME=add_users_table
make migrate-up // update table
make migrate-down // revert table
````⌊倠捡慫敧㩳ਊ搼瑥楡獬ਾ㰉畳浭牡㹹㰠瑳潲杮‾灡数牲牯⁳⼼瑳潲杮‾⼼畳浭牡㹹ਉⴊⴭਊ⌣⌣‣畆据楴湯㩳ਊ⸱嬠习睥畁桴牯穩瑡潩恮⡝⼮捡潣湵⽴潭敤⽬灡数牲牯⽳牥潲獲朮⍯㡌⤱›丠睥畁桴牯穩瑡潩⁮潴挠敲瑡⁥⁡〴਱⸲嬠习睥慂剤煥敵瑳嵠⸨愯捣畯瑮洯摯汥愯灰牥潲獲支牲牯⹳潧䰣㤸㨩†敎䉷摡敒畱獥⁴潴挠敲瑡⁥〴‰牥潲獲⠠慶楬慤楴湯‬潦⁲硥浡汰⥥㌊‮恛敎䍷湯汦捩恴⡝⼮捡潣湵⽴潭敤⽬灡数牲牯⽳牥潲獲朮⍯㥌⤷›丠睥潃普楬瑣琠⁯牣慥整愠⁮牥潲⁲潦⁲〴ਹ⸴嬠习睥湉整湲污嵠⸨愯捣畯瑮洯摯汥愯灰牥潲獲支牲牯⹳潧䰣〱⤵›丠睥湉整湲污映牯㔠〰攠牲牯⁳湡⁤湵湫睯⁮牥潲獲㔊‮恛敎乷瑯潆湵恤⡝⼮捡潣湵⽴潭敤⽬灡数牲牯⽳牥潲獲朮⍯ㅌ㌱㨩†敎乷瑯潆湵⁤潴挠敲瑡⁥湡攠牲牯映牯㐠㐰㘊‮恛敎偷祡潬摡潔䱯牡敧嵠⸨愯捣畯瑮洯摯汥愯灰牥潲獲支牲牯⹳潧䰣㈱⤱›丠睥慐汹慯呤潯慌杲⁥潴挠敲瑡⁥湡攠牲牯映牯㐠㌱㜊‮恛敎卷牥楶散湕癡楡慬汢恥⡝⼮捡潣湵⽴潭敤⽬灡数牲牯⽳牥潲獲朮⍯ㅌ㤲㨩†敎卷牥楶散湕癡楡慬汢⁥潴挠敲瑡⁥湡攠牲牯映牯㔠㌰㠊‮恛敎啷獮灵潰瑲摥敍楤呡灹恥⡝⼮捡潣湵⽴潭敤⽬灡数牲牯⽳牥潲獲朮⍯ㅌ㜳㨩†敎啷獮灵潰瑲摥敍楤呡灹⁥潴挠敲瑡⁥湡攠牲牯映牯㐠㔱㤊‮恛瑓瑡獵嵠⸨愯捣畯瑮洯摯汥愯灰牥潲獲支牲牯⹳潧䰣㠶㨩†瑓瑡獵挠敨正⁳桴⁥畲瑮浩⁥祴数漠⁦桴⁥牥潲⁲湡⁤敲畴湲⁳⁡瑨灴猠慴畴⁳潣敤椠⁦桴⁥牥潲⁲獩洠摯汥䔮牲牯ਊⴭਭ⌣⌣‣祔数ੳㄊ‮恛牅潲恲⡝⼮捡潣湵⽴潭敤⽬灡数牲牯⽳牥潲獲朮⍯㉌⤷›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊⴊⴭ㰊搯瑥楡獬㰾敤慴汩㹳ऊ猼浵慭祲‾猼牴湯㹧栠湡汤牥㰠猯牴湯㹧㰠猯浵慭祲ाਊⴭਭ⌊⌣⌣䘠湵瑣潩獮਺ㄊ‮恛敎䡷湡汤牥嵠⸨愯捣畯瑮栯湡汤牥栯湡汤牥朮⍯㍌⤰›丠睥慈摮敬⁲湩瑩慩楬敺⁳桴⁥慨摮敬⁲楷桴爠煥極敲⁤湩敪瑣摥猠牥楶散⁳污湯⁧楷桴栠瑴⁰潲瑵獥䐠敯⁳潮⁴敲畴湲愠⁳瑩搠慥獬搠物捥汴⁹楷桴愠爠晥牥湥散琠⁯桴⁥楧⁮湅楧敮ਊⴭਭ⌣⌣‣祔数ੳㄊ‮恛潃普杩嵠⸨愯捣畯瑮栯湡汤牥栯湡汤牥朮⍯㉌⤰›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊ⸲嬠䡠湡汤牥嵠⸨愯捣畯瑮栯湡汤牥栯湡汤牥朮⍯ㅌ⤳›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊⴊⴭ㰊搯瑥楡獬㰾敤慴汩㹳ऊ猼浵慭祲‾猼牴湯㹧洠摩汤睥牡⁥⼼瑳潲杮‾⼼畳浭牡㹹ਉⴊⴭਊ⌣⌣‣畆据楴湯㩳ਊ⸱嬠呠浩潥瑵嵠⸨愯捣畯瑮栯湡汤牥洯摩汤睥牡⽥楴敭畯⹴潧䰣ㄸ㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮⴊⴭ㰊搯瑥楡獬㰾敤慴汩㹳ऊ猼浵慭祲‾猼牴湯㹧洠捯獫㰠猯牴湯㹧㰠猯浵慭祲ाਊⴭਭ⌊⌣⌣吠灹獥ਊ⸱嬠䵠捯呫歯湥敒潰楳潴祲嵠⸨愯捣畯瑮洯摯汥洯捯獫琯歯湥牟灥獯瑩牯⹹潧䰣㈱㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮ㈊‮恛潍正潔敫卮牥楶散嵠⸨愯捣畯瑮洯摯汥洯捯獫琯歯湥獟牥楶散朮⍯ㅌ⤰›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊ⸳嬠䵠捯啫敳割灥獯瑩牯恹⡝⼮捡潣湵⽴潭敤⽬潭正⽳獵牥牟灥獯瑩牯⹹潧䰣㈱㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮ㐊‮恛潍正獕牥敓癲捩恥⡝⼮捡潣湵⽴潭敤⽬潭正⽳獵牥獟牥楶散朮⍯ㅌ⤲›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊⴊⴭ㰊搯瑥楡獬㰾敤慴汩㹳ऊ猼浵慭祲‾猼牴湯㹧洠摯汥㰠猯牴湯㹧㰠猯浵慭祲ाਊⴭਭ⌊⌣⌣吠灹獥ਊ⸱嬠䥠呄歯湥畃瑳浯汃楡獭嵠⸨愯捣畯瑮洯摯汥琯歯湥⹳潧䰣㘱㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮ㈊‮恛敒牦獥周歯湥嵠⸨愯捣畯瑮洯摯汥琯歯湥⹳潧䰣㌲㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮ㌊‮恛敒牦獥周歯湥畃瑳浯汃楡獭嵠⸨愯捣畯瑮洯摯汥琯歯湥⹳潧䰣㈳㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮ㐊‮恛潔敫恮⡝⼮捡潣湵⽴潭敤⽬潴敫獮朮⍯ㅌ⤰›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊ⸵嬠啠敳恲⡝⼮捡潣湵⽴潭敤⽬獵牥⹳潧䰣⤸›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊⴊⴭ㰊搯瑥楡獬㰾敤慴汩㹳ऊ猼浵慭祲‾猼牴湯㹧爠灥獯瑩牯⁹⼼瑳潲杮‾⼼畳浭牡㹹ਉⴊⴭਊ⌣⌣‣畆据楴湯㩳ਊ⸱嬠习睥潔敫剮灥獯瑩牯恹⡝⼮捡潣湵⽴敲潰楳潴祲爯摥獩瑟歯湥牟灥獯瑩牯⹹潧䰣〲㨩†敎呷歯湥敒潰楳潴祲椠⁳⁡慦瑣牯⁹潦⁲湩瑩慩楬楺杮唠敳⁲敒潰楳潴楲獥㈊‮恛敎啷敳割灥獯瑩牯恹⡝⼮捡潣湵⽴敲潰楳潴祲瀯獯杴敲彳獵牥牟灥獯瑩牯⹹潧䰣〲㨩†敎啷敳割灥獯瑩牯⁹獩愠映捡潴祲映牯椠楮楴污穩湩⁧獕牥删灥獯瑩牯敩ੳⴊⴭ㰊搯瑥楡獬㰾敤慴汩㹳ऊ猼浵慭祲‾猼牴湯㹧猠牥楶散㰠猯牴湯㹧㰠猯浵慭祲ाਊⴭਭ⌊⌣⌣䘠湵瑣潩獮਺ㄊ‮恛敎呷歯湥敓癲捩恥⡝⼮捡潣湵⽴敳癲捩⽥潴敫⹮潧䰣㜳㨩†敎呷歯湥敓癲捩⁥獩愠映捡潴祲映湵瑣潩⁮潦⁲湩瑩慩楬楺杮愠唠敳卲牥楶散眠瑩⁨瑩⁳敲潰楳潴祲氠祡牥搠灥湥敤据敩ੳ⸲嬠习睥獕牥敓癲捩恥⡝⼮捡潣湵⽴敳癲捩⽥獵牥朮⍯㉌⤶›丠睥獕牥敓癲捩⁥獩愠映捡潴祲映湵瑣潩⁮潦⁲湩瑩慩楬楺杮愠唠敳卲牥楶散眠瑩⁨瑩⁳敲潰楳潴祲氠祡牥搠灥湥敤据敩ੳⴊⴭ⌊⌣⌣吠灹獥ਊ⸱嬠呠歯湥敓癲捩䍥湯楦恧⡝⼮捡潣湵⽴敳癲捩⽥潴敫⹮潧䰣㘲㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮ㈊‮恛单潃普杩嵠⸨愯捣畯瑮猯牥楶散甯敳⹲潧䰣〲㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮਊⴭਭ⼼敤慴汩㹳搼瑥楡獬ਾ㰉畳浭牡㹹㰠瑳潲杮‾瑵汩⁳⼼瑳潲杮‾⼼畳浭牡㹹ਉⴊⴭਊ⌣⌣‣畆据楴湯㩳ਊ⸱嬠䍠浯慰敲慐獳潷摲恳⡝⼮捡潣湵⽴瑵汩⽳慰獳潷摲朮⍯㍌⤲›潎搠獥牣灩楴湯瀠潲楶敤⹤㈊‮恛敇敮慲整䑉潔敫恮⡝⼮捡潣湵⽴瑵汩⽳潴敫⹮潧䰣㔱㨩†敇敮慲整䑉潔敫⁮敧敮慲整⁳湡䤠呄歯湥眠楨档椠⁳⁡睪⁴楷桴洠䍹獵潴䍭慬浩⁳潃汵⁤慣汬琠楨⁳敇敮慲整䑉潔敫卮牴湩Ⱨ戠瑵琠敨猠杩慮畴敲洠歡獥琠楨⁳慦物祬挠敬牡㌊‮恛敇敮慲整敒牦獥周歯湥嵠⸨愯捣畯瑮甯楴獬琯歯湥朮⍯㑌⤰›䜠湥牥瑡剥晥敲桳潔敫⁮牣慥整⁳⁡敲牦獥⁨潴敫⁮桔⁥敲牦獥⁨潴敫⁮瑳牯獥漠汮⁹桴⁥獵牥猧䤠ⱄ愠猠牴湩੧⸴嬠䡠獡偨獡睳牯恤⡝⼮捡潣湵⽴瑵汩⽳慰獳潷摲朮⍯ㅌ⤲›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊⴭਭ⼼敤慴汩㹳⌊倠捡慫敧㩳ਊ搼瑥楡獬ਾ㰉畳浭牡㹹㰠瑳潲杮‾灡数牲牯⁳⼼瑳潲杮‾⼼畳浭牡㹹ਉⴊⴭਊ⌣⌣‣畆据楴湯㩳ਊ⸱嬠习睥畁桴牯穩瑡潩恮⡝⼮捡潣湵⽴潭敤⽬灡数牲牯⽳牥潲獲朮⍯㡌⤱›丠睥畁桴牯穩瑡潩⁮潴挠敲瑡⁥⁡〴਱⸲嬠习睥慂剤煥敵瑳嵠⸨愯捣畯瑮洯摯汥愯灰牥潲獲支牲牯⹳潧䰣㤸㨩†敎䉷摡敒畱獥⁴潴挠敲瑡⁥〴‰牥潲獲⠠慶楬慤楴湯‬潦⁲硥浡汰⥥㌊‮恛敎䍷湯汦捩恴⡝⼮捡潣湵⽴潭敤⽬灡数牲牯⽳牥潲獲朮⍯㥌⤷›丠睥潃普楬瑣琠⁯牣慥整愠⁮牥潲⁲潦⁲〴ਹ⸴嬠习睥湉整湲污嵠⸨愯捣畯瑮洯摯汥愯灰牥潲獲支牲牯⹳潧䰣〱⤵›丠睥湉整湲污映牯㔠〰攠牲牯⁳湡⁤湵湫睯⁮牥潲獲㔊‮恛敎乷瑯潆湵恤⡝⼮捡潣湵⽴潭敤⽬灡数牲牯⽳牥潲獲朮⍯ㅌ㌱㨩†敎乷瑯潆湵⁤潴挠敲瑡⁥湡攠牲牯映牯㐠㐰㘊‮恛敎偷祡潬摡潔䱯牡敧嵠⸨愯捣畯瑮洯摯汥愯灰牥潲獲支牲牯⹳潧䰣㈱⤱›丠睥慐汹慯呤潯慌杲⁥潴挠敲瑡⁥湡攠牲牯映牯㐠㌱㜊‮恛敎卷牥楶散湕癡楡慬汢恥⡝⼮捡潣湵⽴潭敤⽬灡数牲牯⽳牥潲獲朮⍯ㅌ㤲㨩†敎卷牥楶散湕癡楡慬汢⁥潴挠敲瑡⁥湡攠牲牯映牯㔠㌰㠊‮恛敎啷獮灵潰瑲摥敍楤呡灹恥⡝⼮捡潣湵⽴潭敤⽬灡数牲牯⽳牥潲獲朮⍯ㅌ㜳㨩†敎啷獮灵潰瑲摥敍楤呡灹⁥潴挠敲瑡⁥湡攠牲牯映牯㐠㔱㤊‮恛瑓瑡獵嵠⸨愯捣畯瑮洯摯汥愯灰牥潲獲支牲牯⹳潧䰣㠶㨩†瑓瑡獵挠敨正⁳桴⁥畲瑮浩⁥祴数漠⁦桴⁥牥潲⁲湡⁤敲畴湲⁳⁡瑨灴猠慴畴⁳潣敤椠⁦桴⁥牥潲⁲獩洠摯汥䔮牲牯ਊⴭਭ⌣⌣‣祔数ੳㄊ‮恛牅潲恲⡝⼮捡潣湵⽴潭敤⽬灡数牲牯⽳牥潲獲朮⍯㉌⤷›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊⴊⴭ㰊搯瑥楡獬㰾敤慴汩㹳ऊ猼浵慭祲‾猼牴湯㹧栠湡汤牥㰠猯牴湯㹧㰠猯浵慭祲ाਊⴭਭ⌊⌣⌣䘠湵瑣潩獮਺ㄊ‮恛敎䡷湡汤牥嵠⸨愯捣畯瑮栯湡汤牥栯湡汤牥朮⍯㍌⤰›丠睥慈摮敬⁲湩瑩慩楬敺⁳桴⁥慨摮敬⁲楷桴爠煥極敲⁤湩敪瑣摥猠牥楶散⁳污湯⁧楷桴栠瑴⁰潲瑵獥䐠敯⁳潮⁴敲畴湲愠⁳瑩搠慥獬搠物捥汴⁹楷桴愠爠晥牥湥散琠⁯桴⁥楧⁮湅楧敮ਊⴭਭ⌣⌣‣祔数ੳㄊ‮恛潃普杩嵠⸨愯捣畯瑮栯湡汤牥栯湡汤牥朮⍯㉌⤰›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊ⸲嬠䡠湡汤牥嵠⸨愯捣畯瑮栯湡汤牥栯湡汤牥朮⍯ㅌ⤳›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊⴊⴭ㰊搯瑥楡獬㰾敤慴汩㹳ऊ猼浵慭祲‾猼牴湯㹧洠摩汤睥牡⁥⼼瑳潲杮‾⼼畳浭牡㹹ਉⴊⴭਊ⌣⌣‣畆据楴湯㩳ਊ⸱嬠呠浩潥瑵嵠⸨愯捣畯瑮栯湡汤牥洯摩汤睥牡⽥楴敭畯⹴潧䰣ㄸ㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮⴊⴭ㰊搯瑥楡獬㰾敤慴汩㹳ऊ猼浵慭祲‾猼牴湯㹧洠捯獫㰠猯牴湯㹧㰠猯浵慭祲ाਊⴭਭ⌊⌣⌣吠灹獥ਊ⸱嬠䵠捯呫歯湥敒潰楳潴祲嵠⸨愯捣畯瑮洯摯汥洯捯獫琯歯湥牟灥獯瑩牯⹹潧䰣㈱㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮ㈊‮恛潍正潔敫卮牥楶散嵠⸨愯捣畯瑮洯摯汥洯捯獫琯歯湥獟牥楶散朮⍯ㅌ⤰›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊ⸳嬠䵠捯啫敳割灥獯瑩牯恹⡝⼮捡潣湵⽴潭敤⽬潭正⽳獵牥牟灥獯瑩牯⹹潧䰣㈱㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮ㐊‮恛潍正獕牥敓癲捩恥⡝⼮捡潣湵⽴潭敤⽬潭正⽳獵牥獟牥楶散朮⍯ㅌ⤲›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊⴊⴭ㰊搯瑥楡獬㰾敤慴汩㹳ऊ猼浵慭祲‾猼牴湯㹧洠摯汥㰠猯牴湯㹧㰠猯浵慭祲ाਊⴭਭ⌊⌣⌣吠灹獥ਊ⸱嬠䥠呄歯湥畃瑳浯汃楡獭嵠⸨愯捣畯瑮洯摯汥琯歯湥⹳潧䰣㘱㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮ㈊‮恛敒牦獥周歯湥嵠⸨愯捣畯瑮洯摯汥琯歯湥⹳潧䰣㌲㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮ㌊‮恛敒牦獥周歯湥畃瑳浯汃楡獭嵠⸨愯捣畯瑮洯摯汥琯歯湥⹳潧䰣㈳㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮ㐊‮恛潔敫恮⡝⼮捡潣湵⽴潭敤⽬潴敫獮朮⍯ㅌ⤰›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊ⸵嬠啠敳恲⡝⼮捡潣湵⽴潭敤⽬獵牥⹳潧䰣⤸›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊⴊⴭ㰊搯瑥楡獬㰾敤慴汩㹳ऊ猼浵慭祲‾猼牴湯㹧爠灥獯瑩牯⁹⼼瑳潲杮‾⼼畳浭牡㹹ਉⴊⴭਊ⌣⌣‣畆据楴湯㩳ਊ⸱嬠习睥潔敫剮灥獯瑩牯恹⡝⼮捡潣湵⽴敲潰楳潴祲爯摥獩瑟歯湥牟灥獯瑩牯⹹潧䰣〲㨩†敎呷歯湥敒潰楳潴祲椠⁳⁡慦瑣牯⁹潦⁲湩瑩慩楬楺杮唠敳⁲敒潰楳潴楲獥㈊‮恛敎啷敳割灥獯瑩牯恹⡝⼮捡潣湵⽴敲潰楳潴祲瀯獯杴敲彳獵牥牟灥獯瑩牯⹹潧䰣〲㨩†敎啷敳割灥獯瑩牯⁹獩愠映捡潴祲映牯椠楮楴污穩湩⁧獕牥删灥獯瑩牯敩ੳⴊⴭ㰊搯瑥楡獬㰾敤慴汩㹳ऊ猼浵慭祲‾猼牴湯㹧猠牥楶散㰠猯牴湯㹧㰠猯浵慭祲ाਊⴭਭ⌊⌣⌣䘠湵瑣潩獮਺ㄊ‮恛敎呷歯湥敓癲捩恥⡝⼮捡潣湵⽴敳癲捩⽥潴敫⹮潧䰣㜳㨩†敎呷歯湥敓癲捩⁥獩愠映捡潴祲映湵瑣潩⁮潦⁲湩瑩慩楬楺杮愠唠敳卲牥楶散眠瑩⁨瑩⁳敲潰楳潴祲氠祡牥搠灥湥敤据敩ੳ⸲嬠习睥獕牥敓癲捩恥⡝⼮捡潣湵⽴敳癲捩⽥獵牥朮⍯㉌⤶›丠睥獕牥敓癲捩⁥獩愠映捡潴祲映湵瑣潩⁮潦⁲湩瑩慩楬楺杮愠唠敳卲牥楶散眠瑩⁨瑩⁳敲潰楳潴祲氠祡牥搠灥湥敤据敩ੳⴊⴭ⌊⌣⌣吠灹獥ਊ⸱嬠呠歯湥敓癲捩䍥湯楦恧⡝⼮捡潣湵⽴敳癲捩⽥潴敫⹮潧䰣㘲㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮ㈊‮恛单潃普杩嵠⸨愯捣畯瑮猯牥楶散甯敳⹲潧䰣〲㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮਊⴭਭ⼼敤慴汩㹳搼瑥楡獬ਾ㰉畳浭牡㹹㰠瑳潲杮‾瑵汩⁳⼼瑳潲杮‾⼼畳浭牡㹹ਉⴊⴭਊ⌣⌣‣畆据楴湯㩳ਊ⸱嬠䍠浯慰敲慐獳潷摲恳⡝⼮捡潣湵⽴瑵汩⽳慰獳潷摲朮⍯㍌⤲›潎搠獥牣灩楴湯瀠潲楶敤⹤㈊‮恛敇敮慲整䑉潔敫恮⡝⼮捡潣湵⽴瑵汩⽳潴敫⹮潧䰣㔱㨩†敇敮慲整䑉潔敫⁮敧敮慲整⁳湡䤠呄歯湥眠楨档椠⁳⁡睪⁴楷桴洠䍹獵潴䍭慬浩⁳潃汵⁤慣汬琠楨⁳敇敮慲整䑉潔敫卮牴湩Ⱨ戠瑵琠敨猠杩慮畴敲洠歡獥琠楨⁳慦物祬挠敬牡㌊‮恛敇敮慲整敒牦獥周歯湥嵠⸨愯捣畯瑮甯楴獬琯歯湥朮⍯㑌⤰›䜠湥牥瑡剥晥敲桳潔敫⁮牣慥整⁳⁡敲牦獥⁨潴敫⁮桔⁥敲牦獥⁨潴敫⁮瑳牯獥漠汮⁹桴⁥獵牥猧䤠ⱄ愠猠牴湩੧⸴嬠䡠獡偨獡睳牯恤⡝⼮捡潣湵⽴瑵汩⽳慰獳潷摲朮⍯ㅌ⤲›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊⴭਭ⼼敤慴汩㹳⌊倠捡慫敧㩳ਊ搼瑥楡獬ਾ㰉畳浭牡㹹㰠瑳潲杮‾灡数牲牯⁳⼼瑳潲杮‾⼼畳浭牡㹹ਉⴊⴭਊ⌣⌣‣畆据楴湯㩳ਊ⸱嬠习睥畁桴牯穩瑡潩恮⡝⼮捡潣湵⽴潭敤⽬灡数牲牯⽳牥潲獲朮⍯㡌⤱›丠睥畁桴牯穩瑡潩⁮潴挠敲瑡⁥⁡〴਱⸲嬠习睥慂剤煥敵瑳嵠⸨愯捣畯瑮洯摯汥愯灰牥潲獲支牲牯⹳潧䰣㤸㨩†敎䉷摡敒畱獥⁴潴挠敲瑡⁥〴‰牥潲獲⠠慶楬慤楴湯‬潦⁲硥浡汰⥥㌊‮恛敎䍷湯汦捩恴⡝⼮捡潣湵⽴潭敤⽬灡数牲牯⽳牥潲獲朮⍯㥌⤷›丠睥潃普楬瑣琠⁯牣慥整愠⁮牥潲⁲潦⁲〴ਹ⸴嬠习睥湉整湲污嵠⸨愯捣畯瑮洯摯汥愯灰牥潲獲支牲牯⹳潧䰣〱⤵›丠睥湉整湲污映牯㔠〰攠牲牯⁳湡⁤湵湫睯⁮牥潲獲㔊‮恛敎乷瑯潆湵恤⡝⼮捡潣湵⽴潭敤⽬灡数牲牯⽳牥潲獲朮⍯ㅌ㌱㨩†敎乷瑯潆湵⁤潴挠敲瑡⁥湡攠牲牯映牯㐠㐰㘊‮恛敎偷祡潬摡潔䱯牡敧嵠⸨愯捣畯瑮洯摯汥愯灰牥潲獲支牲牯⹳潧䰣㈱⤱›丠睥慐汹慯呤潯慌杲⁥潴挠敲瑡⁥湡攠牲牯映牯㐠㌱㜊‮恛敎卷牥楶散湕癡楡慬汢恥⡝⼮捡潣湵⽴潭敤⽬灡数牲牯⽳牥潲獲朮⍯ㅌ㤲㨩†敎卷牥楶散湕癡楡慬汢⁥潴挠敲瑡⁥湡攠牲牯映牯㔠㌰㠊‮恛敎啷獮灵潰瑲摥敍楤呡灹恥⡝⼮捡潣湵⽴潭敤⽬灡数牲牯⽳牥潲獲朮⍯ㅌ㜳㨩†敎啷獮灵潰瑲摥敍楤呡灹⁥潴挠敲瑡⁥湡攠牲牯映牯㐠㔱㤊‮恛瑓瑡獵嵠⸨愯捣畯瑮洯摯汥愯灰牥潲獲支牲牯⹳潧䰣㠶㨩†瑓瑡獵挠敨正⁳桴⁥畲瑮浩⁥祴数漠⁦桴⁥牥潲⁲湡⁤敲畴湲⁳⁡瑨灴猠慴畴⁳潣敤椠⁦桴⁥牥潲⁲獩洠摯汥䔮牲牯ਊⴭਭ⌣⌣‣祔数ੳㄊ‮恛牅潲恲⡝⼮捡潣湵⽴潭敤⽬灡数牲牯⽳牥潲獲朮⍯㉌⤷›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊⴊⴭ㰊搯瑥楡獬㰾敤慴汩㹳ऊ猼浵慭祲‾猼牴湯㹧栠湡汤牥㰠猯牴湯㹧㰠猯浵慭祲ाਊⴭਭ⌊⌣⌣䘠湵瑣潩獮਺ㄊ‮恛敎䡷湡汤牥嵠⸨愯捣畯瑮栯湡汤牥栯湡汤牥朮⍯㍌⤰›丠睥慈摮敬⁲湩瑩慩楬敺⁳桴⁥慨摮敬⁲楷桴爠煥極敲⁤湩敪瑣摥猠牥楶散⁳污湯⁧楷桴栠瑴⁰潲瑵獥䐠敯⁳潮⁴敲畴湲愠⁳瑩搠慥獬搠物捥汴⁹楷桴愠爠晥牥湥散琠⁯桴⁥楧⁮湅楧敮ਊⴭਭ⌣⌣‣祔数ੳㄊ‮恛潃普杩嵠⸨愯捣畯瑮栯湡汤牥栯湡汤牥朮⍯㉌⤰›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊ⸲嬠䡠湡汤牥嵠⸨愯捣畯瑮栯湡汤牥栯湡汤牥朮⍯ㅌ⤳›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊⴊⴭ㰊搯瑥楡獬㰾敤慴汩㹳ऊ猼浵慭祲‾猼牴湯㹧洠摩汤睥牡⁥⼼瑳潲杮‾⼼畳浭牡㹹ਉⴊⴭਊ⌣⌣‣畆据楴湯㩳ਊ⸱嬠呠浩潥瑵嵠⸨愯捣畯瑮栯湡汤牥洯摩汤睥牡⽥楴敭畯⹴潧䰣ㄸ㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮⴊⴭ㰊搯瑥楡獬㰾敤慴汩㹳ऊ猼浵慭祲‾猼牴湯㹧洠捯獫㰠猯牴湯㹧㰠猯浵慭祲ाਊⴭਭ⌊⌣⌣吠灹獥ਊ⸱嬠䵠捯呫歯湥敒潰楳潴祲嵠⸨愯捣畯瑮洯摯汥洯捯獫琯歯湥牟灥獯瑩牯⹹潧䰣㈱㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮ㈊‮恛潍正潔敫卮牥楶散嵠⸨愯捣畯瑮洯摯汥洯捯獫琯歯湥獟牥楶散朮⍯ㅌ⤰›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊ⸳嬠䵠捯啫敳割灥獯瑩牯恹⡝⼮捡潣湵⽴潭敤⽬潭正⽳獵牥牟灥獯瑩牯⹹潧䰣㈱㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮ㐊‮恛潍正獕牥敓癲捩恥⡝⼮捡潣湵⽴潭敤⽬潭正⽳獵牥獟牥楶散朮⍯ㅌ⤲›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊⴊⴭ㰊搯瑥楡獬㰾敤慴汩㹳ऊ猼浵慭祲‾猼牴湯㹧洠摯汥㰠猯牴湯㹧㰠猯浵慭祲ाਊⴭਭ⌊⌣⌣吠灹獥ਊ⸱嬠䥠呄歯湥畃瑳浯汃楡獭嵠⸨愯捣畯瑮洯摯汥琯歯湥⹳潧䰣㘱㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮ㈊‮恛敒牦獥周歯湥嵠⸨愯捣畯瑮洯摯汥琯歯湥⹳潧䰣㌲㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮ㌊‮恛敒牦獥周歯湥畃瑳浯汃楡獭嵠⸨愯捣畯瑮洯摯汥琯歯湥⹳潧䰣㈳㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮ㐊‮恛潔敫恮⡝⼮捡潣湵⽴潭敤⽬潴敫獮朮⍯ㅌ⤰›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊ⸵嬠啠敳恲⡝⼮捡潣湵⽴潭敤⽬獵牥⹳潧䰣⤸›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊⴊⴭ㰊搯瑥楡獬㰾敤慴汩㹳ऊ猼浵慭祲‾猼牴湯㹧爠灥獯瑩牯⁹⼼瑳潲杮‾⼼畳浭牡㹹ਉⴊⴭਊ⌣⌣‣畆据楴湯㩳ਊ⸱嬠习睥潔敫剮灥獯瑩牯恹⡝⼮捡潣湵⽴敲潰楳潴祲爯摥獩瑟歯湥牟灥獯瑩牯⹹潧䰣〲㨩†敎呷歯湥敒潰楳潴祲椠⁳⁡慦瑣牯⁹潦⁲湩瑩慩楬楺杮唠敳⁲敒潰楳潴楲獥㈊‮恛敎啷敳割灥獯瑩牯恹⡝⼮捡潣湵⽴敲潰楳潴祲瀯獯杴敲彳獵牥牟灥獯瑩牯⹹潧䰣〲㨩†敎啷敳割灥獯瑩牯⁹獩愠映捡潴祲映牯椠楮楴污穩湩⁧獕牥删灥獯瑩牯敩ੳⴊⴭ㰊搯瑥楡獬㰾敤慴汩㹳ऊ猼浵慭祲‾猼牴湯㹧猠牥楶散㰠猯牴湯㹧㰠猯浵慭祲ाਊⴭਭ⌊⌣⌣䘠湵瑣潩獮਺ㄊ‮恛敎呷歯湥敓癲捩恥⡝⼮捡潣湵⽴敳癲捩⽥潴敫⹮潧䰣㜳㨩†敎呷歯湥敓癲捩⁥獩愠映捡潴祲映湵瑣潩⁮潦⁲湩瑩慩楬楺杮愠唠敳卲牥楶散眠瑩⁨瑩⁳敲潰楳潴祲氠祡牥搠灥湥敤据敩ੳ⸲嬠习睥獕牥敓癲捩恥⡝⼮捡潣湵⽴敳癲捩⽥獵牥朮⍯㉌⤶›丠睥獕牥敓癲捩⁥獩愠映捡潴祲映湵瑣潩⁮潦⁲湩瑩慩楬楺杮愠唠敳卲牥楶散眠瑩⁨瑩⁳敲潰楳潴祲氠祡牥搠灥湥敤据敩ੳⴊⴭ⌊⌣⌣吠灹獥ਊ⸱嬠呠歯湥敓癲捩䍥湯楦恧⡝⼮捡潣湵⽴敳癲捩⽥潴敫⹮潧䰣㘲㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮ㈊‮恛单潃普杩嵠⸨愯捣畯瑮猯牥楶散甯敳⹲潧䰣〲㨩丠⁯敤捳楲瑰潩⁮牰癯摩摥ਮਊⴭਭ⼼敤慴汩㹳搼瑥楡獬ਾ㰉畳浭牡㹹㰠瑳潲杮‾瑵汩⁳⼼瑳潲杮‾⼼畳浭牡㹹ਉⴊⴭਊ⌣⌣‣畆据楴湯㩳ਊ⸱嬠䍠浯慰敲慐獳潷摲恳⡝⼮捡潣湵⽴瑵汩⽳慰獳潷摲朮⍯㍌⤲›潎搠獥牣灩楴湯瀠潲楶敤⹤㈊‮恛敇敮慲整䑉潔敫恮⡝⼮捡潣湵⽴瑵汩⽳潴敫⹮潧䰣㔱㨩†敇敮慲整䑉潔敫⁮敧敮慲整⁳湡䤠呄歯湥眠楨档椠⁳⁡睪⁴楷桴洠䍹獵潴䍭慬浩⁳潃汵⁤慣汬琠楨⁳敇敮慲整䑉潔敫卮牴湩Ⱨ戠瑵琠敨猠杩慮畴敲洠歡獥琠楨⁳慦物祬挠敬牡㌊‮恛敇敮慲整敒牦獥周歯湥嵠⸨愯捣畯瑮甯楴獬琯歯湥朮⍯㑌⤰›䜠湥牥瑡剥晥敲桳潔敫⁮牣慥整⁳⁡敲牦獥⁨潴敫⁮桔⁥敲牦獥⁨潴敫⁮瑳牯獥漠汮⁹桴⁥獵牥猧䤠ⱄ愠猠牴湩੧⸴嬠䡠獡偨獡睳牯恤⡝⼮捡潣湵⽴瑵汩⽳慰獳潷摲朮⍯ㅌ⤲›潎搠獥牣灩楴湯瀠潲楶敤⹤ਊⴭਭ⼼敤慴汩㹳�