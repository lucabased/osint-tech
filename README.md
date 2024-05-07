# What?
 * This repo is used for later reference and archival of techniques.
 * The tools and techniques listed here have proven very effective for me in the past.
 * The geographic scope of targets is on Germany.
 * Feel free to contribute to this project.

# IRL-INT ;D
  * Handelsregister/Commercial registry (https://handelsregister.de)
      * Despite the strict national and EU regulations regarding data protection, this technique provides a lot of intelligence about a person and their business associates.
      * Information includes (not limited to): Full legal name, date of birth (DOB), place of birth, addresses, pen signature, marital status, balance sheets, and historic documents of before mentioned things.
      * You'll need to know German in order to read those documents, alternative use a PDF translation service (e.g. Google Lens)
      * Associated people could include venture partners and close family.
      * Usage:
         * Be sure to click the "DK" (ger. Dokumentenansicht) button on the results page.
       
  

# Username
  * Sherlock
      * It's generally good to have an IP from the european nations (e.g. DE, AT, NL)
      * Some results can implicate false-positives due to wrong HTTP status codes provided by the targetted services (e.g. HTTP200 instead of HTTP404)
      * Installation via pipx: `pipx install sherlock`
   
  *     

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
