<div align="center">

## Report Players (Report Panel)

<img src="https://i.imgur.com/LPsTt48.png"></img>

</div>

<p align="center">
  <a href="#requirements">Wymagania ℹ</a> ×
  <a href="#description">Opis 📄</a> ×
  <a href="#configure">Konfiguracja 🛠</a> ×
  <a href="#help">Pomoc 👀</a> ×
  <a href="#screenshots">Screenshot 📷</a>
</p>

---


### Description 
- Zintegrowany z Discord'em system zgłoszenia graczy
- Plugin po wybraniu gracza oraz powodu wysyła wiadomość na nasz serwer Discord, oznaczając przy tym administrację serwera
- Powody zgłoszeń można edytować przez plik `reasons.ini`
- Plugin posiada rozbudowaną opcje konifugracji (40 cvarów)

### Configure
<details>
  <summary><b>report.cfg</b></summary>

```cfg
// Scieżka do pliku z powodami zgłoszeń
amxx4u_report_path "addons_configs/amxx4u/report/reasons.ini"

// Ilość sekund przed kolejnym zgłoszeniem?
amxx4u_report_interval "300.0"

// Maksymalna ilość powodów zgłoszeń
amxx4u_report_maxreason "16"

// Nazwa webhooka z pliku api.cfg
amxx4u_report_webhook "report"

// Jaką flage musi posiadać admin, żeby otrzymać info o zgłoszeniu?
amxx4u_report_flag "d"

// Możliwość zgłaszania adminów?
amxx4u_report_admin "1"

// Pokazywać * przy adminie w menu zgłoszeń?
amxx4u_show_admin "1"

// Pokazywać czas zgłoszenia?
amxx4u_show_time "1"

// Pokazywać mape zgłoszenia?
amxx4u_show_map "1"

// Pokazywać powód zgłoszenia?
amxx4u_show_reason "1"

// Pokazywać zgłoszonego gracza?
amxx4u_show_submitter "1"

// Pokazywać gracza, który zgłosił?
amxx4u_show_reported "1"

// Ustawiać nazwę bota?
amxx4u_show_botname "1"

// Ustawiać avatar bota?
amxx4u_show_avatarbot "1"

// Ustawiać tytuł wiadomości?
amxx4u_show_title "1"

// Ustawiać link po kliknięciu w tytuł?
amxx4u_show_title_url "1"

// Ustawić nazwę autora
// https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_author.png?raw=true
amxx4u_show_author_name "1"

// Pokazywać avatar przy autorze
// https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_author_avatar.png?raw=true
amxx4u_show_avatar_author "1"

// Ustawiać link po kliknięciu w autora?
amxx4u_show_avatar_url "1"

// Powiadamiać adminów o zgłoszeniu (ping roli)
amxx4u_show_ping "1"

// Pokazywać grafikę w thumbnail?
amxx4u_show_thumb "0"

// Pokazywać grafikę nad footerem?
amxx4u_show_embed_img "1"

// Pokazywać tekst w footer?
amxx4u_show_footer_txt "1"

// Pokazywać grafikę przy tekscie w footerze?
amxx4u_show_footer_img "1"

// Nazwa bota na serwerze DC 
// https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_botname.png?raw=true
amxx4u_report_botname "AMXX4u.pl"

// Link do avatara bota
// https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_botavatar.png?raw=true
amxx4u_report_bot_avatar "https://i.imgur.com/3bv7oD8.png"

// Tytuł wiadomości, znajdujący się pod autorem 
// https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_title.png?raw=true
amxx4u_report_title "AMXX4u.pl - Report"

// Link do strony, na która ma admin zostać przekierowany po kliknięciu na tytuł
amxx4u_report_title_url "https://discord.amxx4u.pl/"

// ID Grup które mają zostać oznaczone przy zgłoszeniu
amxx4u_report_content "<@&1031338018583367691>"

// Autor wiadomości, znajdujący się nad tytułem wiadomości
// https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_author.png?raw=true
amxx4u_report_author "Report Panel"

// Link do avatara autora
// https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_author_avatar.png?raw=true
amxx4u_report_author_avatar "https://i.imgur.com/3bv7oD8.png"

// Link do strony, która przekieruje po kliknięciu na autora
amxx4u_report_author_url "https://amxx4u.pl/"

// Tekst znajdujący się w stopce
// https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_footertxt.png?raw=true
amxx4u_report_footer_txt "© AMXX4u.pl"

// Link do grafiki znadującej się przy tekscie w stopce
// https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_footerimg.png?raw=true
amxx4u_report_footer_img "https://i.imgur.com/Y1WyTPw.png"

// Link do grafiki thumbnail
// https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_thumbnail.png?raw=true
amxx4u_report_thumb "https://i.imgur.com/8eok2qn.png"

// Link do grafiki znajdującej sie nad stopką
// https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_mainimg.png?raw=true
amxx4u_report_img "https://i.imgur.com/llAWOkJ.png"
```
</details>

<details>
  <summary><b>reasons.ini</b></summary>

```ini
Cheater
Przeszkadza w grze
Mikro
Troll
```
</details>

<details>
  <summary><b>api.cfg</b></summary>

```json
"Discord"
{
  "report" "https://discord.com/webhook"
}
```
</details>

### Help
<details>
  <summary><b>Author</b></summary>
  <img src="https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_author.png"></img>
</details>

<details>
  <summary><b>Author Avatar</b></summary>
  <img src="https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_author_avatar.png"></img>
</details>

<details>
  <summary><b>BOT Avatar</b></summary>
  <img src="https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_botavatar.png"></img>
</details>

<details>
  <summary><b>BOT Name</b></summary>
  <img src="https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_botname.png"></img>
</details>

<details>
  <summary><b>Embed Title</b></summary>
  <img src="https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_title.png"></img>
</details>

<details>
  <summary><b>Footer Image</b></summary>
  <img src="https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_footerimg.png"></img>
</details>

<details>
  <summary><b>Footer Text</b></summary>
  <img src="https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_footertxt.png"></img>
</details>

<details>
  <summary><b>Embed Thumbnail</b></summary>
  <img src="https://github.com/AMXX4u/Report-players/blob/main/assets/help/help_thumbnail.png"></img>
</details>

### Screenshots

<details>
  <summary><b>Discord</b></summary>

- Main

  <img src="https://github.com/AMXX4u/Report-players/blob/main/assets/discord/none_thumb_dc.png"></img>

- Full

  <img src="https://github.com/AMXX4u/Report-players/blob/main/assets/discord/full_dc.png"></img>
</details>

<details>
  <summary><b>Server:</b></summary>
  
- Admin chat info

  <img src="https://github.com/AMXX4u/Report-players/blob/main/assets/server/admin_chat_info.png"></img>

- Player chat info

  <img src="https://github.com/AMXX4u/Report-players/blob/main/assets/server/player_chat_info.png"></img>
  
- Full chat info

  <img src="https://github.com/AMXX4u/Report-players/blob/main/assets/server/full_chat_info.png"></img>
  
- Cooldown info

  <img src="https://github.com/AMXX4u/Report-players/blob/main/assets/server/cooldown.png"></img>
  
- Menu Players

  <img src="https://github.com/AMXX4u/Report-players/blob/main/assets/server/menu_players.png"></img>
  
- Menu Reasons

  <img src="https://github.com/AMXX4u/Report-players/blob/main/assets/server/menu_reason.png"></img>
</details>


### Requirements 
- AMXModX 1.9 / AMXModX 1.10
- ReHLDS 3.12.0.780
- GRIP 0.1.5
