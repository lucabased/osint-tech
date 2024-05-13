# What?
 * This repo is used for later reference and archival of techniques.
 * The tools and techniques listed here have proven very effective for me in the past.
 * The geographic scope of targets is on Germany.
 * Feel free to contribute to this project.

# CTFs
 * [Sector](https://sector035.n)
 * https://ctf.michweb.de/confirm

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
            * 

        
# Username 
  * Sherlock (https://github.com/sherlock-project/sherlock)
      * It's generally good to have an IP from the european nations (e.g. DE, AT, NL)
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

