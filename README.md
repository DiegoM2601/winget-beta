# Notepad++ es Seguro

El 2 de febrero de 2026, el desarrollador de Notepad++ (Don Ho) confirmó que el mecanismo de actualización automática (WinGup/GUP.exe) había sido comprometido por un grupo de hackers vinculado al gobierno chino (identificado por Rapid7 como "Lotus Blossom"). No fue Notepad++ como programa el que estaba infectado, sino que atacantes lograron acceso a la infraestructura del proveedor de hosting que usaba el sitio web, y desde ahí redirigían selectivamente el tráfico de actualización de ciertos usuarios hacia servidores maliciosos que entregaban instaladores troyanizados. Todo empezó a raíz de la versión 8.8.9, lanzada el 9 de diciembre, que ya venía "endurecida" verificando firma y certificado de los instaladores descargados durante la actualización.

**Lo importante:** Fue un ataque muy selectivo dirigido a usuarios de alto valor específico, no algo masivo, y la mayoría de los usuarios de Notepad++ nunca se vieron afectados, ya que los atacantes filtraban a sus víctimas según valor estratégico, no de forma aleatoria. [The Hacker News](https://thehackernews.com/2026/02/notepad-official-update-mechanism.html)[Notepad++](https://notepad-plus-plus.org/news/clarification-security-incident/)

**¿Ya se solucionó?**

- Se migró el sitio web de Notepad++ a un nuevo proveedor de hosting con prácticas de seguridad mucho más sólidas, y WinGup fue reforzado desde la versión 8.8.9 para verificar tanto el certificado como la firma del instalador descargado. [Notepad++](https://notepad-plus-plus.org/news/hijacked-incident-info-update/)
- El 18 de febrero de 2026 salió la versión 8.9.2, con un proceso de actualización rediseñado tipo "doble candado" que incluye validación por firma XML e instalador firmado, descrito como mucho más resistente a este tipo de explotación. [Hive Systems](https://www.hivesystems.com/blog/when-trusted-tools-are-hijacked-lessons-from-the-notepad-updater-attack)
- El propio Don Ho concluyó: "con estos cambios y refuerzos, creo que la situación se ha resuelto por completo".



---

Fuente: https://www.reddit.com/r/notepadplusplus/comments/1trm8kl/is_notepad_safe_to_use_now/

The hack against Notepad++ was very specifically targeted. The 
program itself was not compromised; the web host for the domain was 
compromised causing upgrades for a very few, chosen companies to be 
redirected to install malware. The chances that any ordinary individual 
was affected are very slim, and the date you list is not within the time
 range of compromise. (See https://notepad-plus-plus.org/news/hijacked-incident-info-update/ and https://notepad-plus-plus.org/news/clarification-security-incident/ for some more information.)

My personal suggestion is to** avoid both auto-upgrade and the web site** and either **download from [GitHub](https://github.com/notepad-plus-plus/notepad-plus-plus/releases) or use [WinGet](https://github.com/microsoft/winget-cli).**

There is a current kerfuffle going on about a couple recent CVEs, 
which are addressed in the latest version of Notepad++, 8.9.6.1; see [discussion here](https://community.notepad-plus-plus.org/topic/27548/notepad-release-8.9.6.1).
 Honestly, some of these recent CVEs are absurd; they amount to “this 
front door is a security risk, because if you leave it unlocked, someone
 could get in.” (These last amount to, if an attacker can modify your 
AppData folder, you can be induced to run malware. If an attacker can 
access your AppData folder, you are already compromised. There might be 
some weird corner case where this could be exploited, but it’s of no 
relevance to ordinary users. Notepad++ has, none-the-less, addressed it,
 but in the process introduced an annoyance for some users which they 
are still working out how to mitigate.)



# LibreOffice

La migración de archivedownload.documentfoundation.org a download.documentfoundation.org es **legítima**.






