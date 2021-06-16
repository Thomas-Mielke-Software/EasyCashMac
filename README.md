# EasyCashMac
ein build environment, um das EasyCash&amp;Tax Codeweavers PortJump Paket für MacOS zu pflegen

## Voraussetzungen
- git large file storage extension
  - geh auf https://git-lfs.github.com und installiere die Extension entsprechend deiner Vorlieben (z.B. 'brew install git-lfs' auf MacOS)
  - ``git lfs install``
- eine passende Developer ID und MacOS distribution provisioning für die AppID- auf https://developer.apple.com .

## Konfigurieren

Das script braucht eine Konfigurationsdatei für die Apple-IDund dein "app-specific password", dasdu dir  auf https://appleid.apple.com erzeugt hast, z.B.:

    echo "appleid=meine@apple.id\naspw=abcd-efgh-ijkl-mnop" > myappleid.config

Optional sollte auch der Wert ascprov= angegeben werden, wenn man als Apple Developer in mehreren Teams ist. Die Konfigurationsdatei sollte dann in etwa so aussehen:

    appleid=mielket@gnx.de
    aspw=qwer-tzui-asdf-ghjk
    ascprov=9Y63EZ54MD

## Bauen

Starten des Build-Scripts:

    ./build.sh

Das sollte im Projektverzeichnis ein Zip-Archiv namens 'EasyCT4Mac.zip' erzeugen, das auf MacOS umstandslos zu öffnen ist.
