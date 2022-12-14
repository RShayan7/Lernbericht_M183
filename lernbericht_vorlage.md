# Lern-Bericht
Shayanthan Ravindran

## Einleitung

Wir befinden uns im Modul 183. In diesem Modul lernen wir über mögliche Hacking angriffe und vertiefen unser gelerntes Wissen über JSF.

## Was habe ich gelernt?
In diesem Lernbericht möchte ich über die "Session Pinning" Methode sprechen, die zu den vielen Hacking-Methoden gehört, die ich gelernt habe.

## Beschreibung
Bei Session Fixation handelt es sich um einen Angriff, bei dem ein Angreifer in der Lage ist, die Sitzung eines Benutzers zu übernehmen. Dieser Angriff nutzt Schwachstellen in der Art und Weise aus, wie bestimmte Webanwendungen die Sitzungs-IDs verwalten. Insbesondere kann es vorkommen, dass bei der Authentifizierung eines Benutzers keine neue Sitzungs-ID erstellt wird, sodass es möglich ist, eine vorhandene Sitzungs-ID zu verwenden. Der Angreifer kann sich also eine gültige Sitzungsnummer beschaffen und versuchen, den Benutzer dazu zu bringen, sich mit dieser Nummer anzumelden. Anschließend kann er die vom Benutzer bestätigte Sitzung durch Kenntnis der verwendeten Sitzungsnummer übernehmen.


```
http://localhost:8080/InsecureApp/faces/secured/index.xhtml;jsessionid=72c5b926347ed646e82d475132dc
```
Wenn ein böser Hacker bsp. in den Besitz von diesem Session Link gelangen könnte, nachdem der Benutzer sich angemeldet hat, könnte er Zugriff auf Daten des Benutzers erlangen. Dieses Problem kann jedoch gelöst werden. 

Die Standardmethode besteht darin, die Sitzungs-ID unmittelbar nach der Anmeldung des Benutzers zu ändern, um die meisten Schwachstellen bei der Sitzungsfixierung zu beseitigen.

Zusätzlich sollten Sitzungs-IDs nach einer bestimmten Zeit ablaufen. Dadurch bleibt dem Angreifer nur ein kleines Zeitfenster, in dem er die feste Sitzungs-ID nutzen kann. 

![image](https://www.checkmarx.com/wp-content/uploads/2016/02/SF.jpg)


![Sessionid](https://user-images.githubusercontent.com/89385736/207733172-7a4fcd7d-5d7a-4650-b000-e874f3f79832.JPG)



## Verifikation

Aus dem kurzen Erklärungstext zum Session Pinning geht hervor, dass ich das Verfahren verstanden habe, bei dem eine unsichere Seite ein Passwort vom Benutzer oder lieber vom Administrator erhält.

# Reflektion zum Arbeitsprozess

Ich bin mit meiner Arbeit nicht so zufrieden. Da ich die ersten zwei Male vom Unterricht verpasst habe, war mir der Einstieg ein wenig schwer. Ich musste viel nacharbeiten und kam mit dem Tempo nicht ganz mit. Ich muss mir klare Ziele setzen für die nächsten Module oder auch bei verpasstem Unterricht. 

👍 Das Gute daran war, dass ich viele neue Begriffe lernen konnte, was mir das Verständnis in diesem Modul ein wneig vereinfachte.

👎 Ich hatte lange für diesen Auftrag gebraucht, da ich die ersten zwei Male vom Unterricht verpasst habe und somit den Einstieg verpasst habe.

**VBV**: Ich werde bei neueren Aufträgen mehr zuhören und bei Unklarheiten den Lehrer fragen. Durch diesen Verbesserungsvorschlag werde ich beim nächsten Mal sicherlich gut vorankommen.



