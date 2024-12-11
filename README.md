# What?
 * This repo is used for later reference and archival of techniques.
 * The tools and techniques listed here have proven very effective for me in the past.
 * The geographic scope of targets is on Germany.
 * Feel free to contribute to this project.

# CTFs
 * [Sector](https://sector035.n)
 * https://ctf.michweb.de/confirm

# Good Resources
 * [Michael Bazzel's OSINT Techniques](https://inteltechniques.com/book1.html)
   
# Visualization / Intel management
 * [Collection of visualized attack surfaces](https://github.com/OsintDojo/OSINT/tree/master)
 * Every great investigation is managed and documented carefully. To retrace steps, find loose ends and being able to get a feel for the bigger picture.
 * Maltego - Community Edition
 * Diagrams.net
 * Obsidian Notebook

# Corporate 
  * Handelsregister/Commercial registry (https://handelsregister.de)
      * Despite the strict national and EU regulations regarding data protection, this technique provides a lot of intelligence about a person and their business associates.
      * Information includes (not limited to): Full legal name, date of birth (DOB), place of birth, addresses, pen signature, marital status, balance sheets, and historic documents of before mentioned things.
      * You'll need to know German in order to read those documents, alternatively use a PDF translation service (e.g. Google Lens)
      * Associated people could include venture partners and close family.
      * Usage:
         * Be sure to click the "DK" (ger. Dokumentenansicht) button on the results page.
         * Archive all of of those documents accordingly in your investigation file.
      * But wait! There are some quicker alternatives than the good ol' Handelsregister.
         * OffeneRegister (https://db.offeneregister.de/)
            * Scraped by some hournorable opendata enthusiasts, this data well can be downloaded.
            * You can now directly search by: partial names, date of birth, address, 
         * Northdata (https://northdata.de/)
            * This service has indexed over 59 million companies in 15 countries as of early May 2024.
            * The free version provides a beautiful network view and semantic connections between other companies and people. This can be extremely useful, as Handelsregister and OpenRegister do not provide this functionality that easily.
            * I'd prefer this over the raw data from Handelsregister, but there is some information that can only be aquired on Handelsregister.
            * Professional version can be obtained by creating a blog.

# Amateurfunker-Rufzeichen
 * The all calling codes are public in Germany (Full name, Adress, Calling code).
 * You can find them there: https://data.bundesnetzagentur.de/Bundesnetzagentur/SharedDocs/Downloads/DE/Sachgebiete/Telekommunikation/Unternehmen_Institutionen/Frequenzen/Amateurfunk/Rufzeichenliste/rufzeichenliste_afu.pdf

# Personal Websites
  * In Germany, there is a law commanding every operator of a website to include an imprint (§5 TMG | https://www.gesetze-im-internet.de/tmg/__5.html)
  * Some people use a masking service such as Autorenglück.de, which invalidates the imprint for us.


# Username 
  * Sherlock (https://github.com/sherlock-project/sherlock)
      * It's generally good to have an IP from the european nations (e.g. DE, AT, NL)
      * Because Sherlock scrapes the websites, I advise you to use a *residential rotating proxy* service such as IPRoyal or PIAProxy
      * Some results can implicate false-positives due to wrong HTTP status codes provided by the targetted services (e.g. HTTP200 instead of HTTP404)
      * Installation via pipx: `pipx install sherlock`
        

# E-mail
  * Holehe (https://github.com/megadose/holehe)
      * Checks multiple websites for an existing registration via the password reset functionality.
      * Can be very noisy.


# Phone number
 * Ignorant (https://github.com/megadose/ignorant)
     * Checks multiple platforms (Amazon, Instagram, Snapchat) for registrations.
     * Can also be very noisy.
  
       
# Data breach (Username, email, password)
  * Dehashed (https://dehashed.com/)
  * 0t.rocks (https://search.0t.rocks)
  * HaveIBeenPwned (https://haveibeenpwned.com/)
  * Snusbase (https://snusbase.com/)
      * 16,5B rows (31.05.2024)
      * My go-to tool for investigating e-mails and usernames.
      * Costs 7 USD/week
      * API endpoint with subscription   
  * CheckLeaked (https://checkleaked.cc)
  * Ghostproject.fr (https://ghostproject.fr/)
    * 15,5B rows (31.05.2024)
    * Does not remove data (suspect does can't hide his trail)
    * 30 USD/month
    * Might be broken  


# Stealer Logs
 * StealerLog Telegram Superlist (https://github.com/fastfire/deepdarkCTI/blob/main/telegram_infostealer.md)
 * Threat actors often archive logs in RAR extensions. This can be dangerous because the RAR protocol contains a few security vulnerabilities leading to RCE. Therefore, it is advised to be only unpacked within a virtual machine that does not contain any sensible information or network access. => Keep a sandbox image at hand :^)


    
# Google / YouTube
  * GHunt (https://github.com/mxrch/GHunt)
      * Aggregate data from all Google services for an account. This includes (not limited to) YouTube, Maps Reviews (A-tier intel), and Google Plus 
      * Authentication via GHunt Companion browser addon (https://addons.mozilla.org/de/firefox/addon/ghunt-companion/)
      * Installation via pipx: `
         pip3 install pipx  &&
         pipx ensurepath &&
         pipx install ghunt`

* yt-dlp (https://github.com/yt-dlp/yt-dlp [fork of yt-dl])
    * Used to scrape comments, account discussions and videos for archival/evidence.
    * Dump meta&comments: `yt-dlp --dump-single-json URL`
    * Installation via AUR repository: `yay -S yt-dlp`
    *  

