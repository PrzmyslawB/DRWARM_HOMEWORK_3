# DRWARM_HOMEWORK_3

#TYDZIEN3.1 „Zbuduj prostą konwencję nazewniczą dla min. takich zasobów jak Grupa Zasobów, VNET, Maszyn Wirtualna, Dysk, Konta składowania danych. Pamiętaj o ograniczeniach w nazywaniu zasobów, które występują w Azure”

Dokumentacja:

https://docs.microsoft.com/en-us/azure/architecture/best-practices/naming-conventions
https://github.com/toddkitta/azure-content/blob/master/articles/guidance/guidance-naming-conventions.md


Grupy zasobów

`<service-short-name>-<environment>-rg-<number>`

- service-short-name - skrócona nazwa usługi,
- environment - środowisko (prod, staging, test, dev, exp),
- number - numer grupy,

Sieci wirtualne

`<service-short-name>-vnet<number>`

- service-short-name - skrócona nazwa sieci,
- number - numer sieci wirtualnej,

Maszyny wirtualne

`<name>-<role>-vm-<number>`

- name - nazwa maszyny,
- role - rola danej maszyny - przeznaczenie,
- number - numer maszyny,

Dyski

`<vm-name>-disk`

- vm-name - nazwa maszyny wirtualnej, do której przypisany jest dysk,
- disk - nazwa dysku,

Konta składowania danych

`<short-service-name>-<role>-st-<number>`

- service-short-name - skrócona nazwa usługi,
- role - rola czyli do czego służy nam konto,
- number - numer konta,

#TYDZIEN3.2 „ Zbuduj prosty ARM Template (możesz wykorzystać już gotowe wzorce z GitHub), który wykorzystuje koncepcję Linked Templates. Template powinien zbudować środowisko złożone z jednej sieci VNET, podzielonej na dwa subnety. W każdy subnecie powinna powstać najprostsza maszyna wirtualna z systemem Ubuntu 18.04 a na każdym subnecie powinny zostać skonfigurowane NSG.”

#TYDZIEN3.3 „Zbuduj najprostrzą właśną rolę RBAC, która pozwala użytkownikowi uruchomić maszynę, zatrzymać ją i zgłosić zgłoszenie do supportu przez Portal Azure”

#TYDZIEN3.4 „Spróbuj na koniec zmodyfikować template tak, by nazwa użytkownika i hasło do każdej maszyny z pkt. 2 było pobierane z KeyVault.„
