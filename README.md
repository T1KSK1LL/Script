// РўСѓС‚РѕСЂРёР°Р» РєР°Рє РЅР°СЃС‚СЂРѕРёС‚СЊ СЃРєСЂРёРїС‚ СЃРјРѕС‚СЂРё РЅР° РєР°РЅР°Р»Рµ 
var kup = Point.get(1108,314); //РєСѓРїРёС‚СЊ
var pod = Point.get(669,520); //РїРѕРґС‚РІРµСЂРґРёС‚СЊ
var gal = Point.get(466,243); //РіР°Р»РѕС‡РєР°
var krest = Point.get(949,247); //РєСЂРµСЃС‚ Сѓ Р»РѕС‚Р°
var osm = Point.get(1213,66); //РІС‹Р№С‚Рё РёР· РѕСЃРјРѕС‚СЂР°
var ok = Point.get(637,510); //РѕРє
var opr = Point.get(942,306); //РћРџР 
int colo2 = 17035; //С†РІРµС‚ РіР°Р»РѕС‡РєРё
int colo = 6447699; //С†РІРµС‚ РѕРїСЂР°
int upd = 15000; //СЃРєРѕСЂРѕСЃС‚СЊ РѕР±РЅРѕРІР»РµРЅРёСЏ

log("Р›СѓС‡С€РёР№ Р‘Р•РЎРџР›РђРўРќР«Р™ РЎРєСЂРёРїС‚ РѕС‚ @T1kSk1ll");
startScreenCapture(2);
var L1 = Point.get();
var L2 = Point.get();
long time = Time.getMillis();
while(!EXIT){  
if(getColor(opr) == colo){
click(kup); sleep(14);
click(pod);sleep(700);
click(krest);sleep(700);
click(ok);sleep(700);
click(osm);sleep(700);
click(gal);sleep(100);
click(gal);sleep(1000);
}
if((Time.getMillis() - time) > upd){
click(gal); sleep(50);
click(gal);
time = Time.getMillis();
sleep(200);
if(getColor(gal) == colo2){
click(gal); sleep(150);  
}
}
}
