# Meter Monitoring System (MMS)

## Taust

Tellijaks on tuntud kindlustusfirma.

Eesmärgiks jälgida tavapärast tarbimist ning tuvastada sellest kõrvalekaldeid (lekkeid) ja nendest siis klientidele (sms,whatsapp)/kindlustusfirmale(email) teada anda.

Meie riistvara osakond on realiseerinud kaamera, mis kinnitatakse mõõdikule. Kaamera saadab perioodiliselt pilti seadistatud IP aadressile.


## Ülesanne

* Lahenduse kirjeldus
	* Esmane serveri komponentmudel
* Keerulised kohad
* Esmane ajahinnang komponentidele

## Flow

´´´mermaid
sequenceDiagram

loop Measure
	Camera->>Camera: Take photo
    Camera->>Server: Send photo
	Server->>User: Notify
	Note right of Server: In case of leakage
end
´´´
