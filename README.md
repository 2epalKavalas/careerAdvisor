# Εικονικός Βοηθός ΣΕΠ
Ανάπτυξη ενός εικονικού βοηθού με αντικείμενο τον Σχολικό Επαγγελματικό Προσανατολισμό (ΣΕΠ)
## [6oς Πανελλήνιος Διαγωνισμός Ανοιχτών Τεχνολογιών](https://openedtech.ellak.gr/) 
### Ομάδα: Τι θα γίνω όταν μεγαλώσω
### Σχολείο: 2ο ΕΠΑΛ Καβάλας (Εσπερινό)
### Μαθητές:
Θωμαΐδου Ελένη, Κοντογιάννης Ιωάννης, Πετρόπουλος Ηρακλής
## Ιδέα
Μετά από συζήτηση στη τάξη και μελέτη διάφορων προτάσεων καταλήξαμε στην πρόταση της δημιουργίας ενός εικονικού βοηθού ΣΕΠ. 
### Υπάρχουσα κατάσταση
Ο θεσμός του ΣΕΠ υποστηρίζεται στην Δευτεροβάθμια Εκπαίδευση μέσω των υπευθύνων ΣΕΠ ανά ΔΔΕ. Παράλληλα σχεδόν κάθε χρόνο αποστέλλονται οδηγίες από το ΙΕΠ για την εφαρμογή του ΣΕΠ στην Γ γυμνασίου για την εφαρμογή του στο πλαίσιο των Εργαστηρίων Δεξιοτήτων. Ο Επαγγελματικός προσανατολισμός είναι ένα πολύ σημαντικό ζήτημα και καθοριστικό για την μετέπειτα πορεία στην ζωή του κάθε μαθητή
### Προβλήμα – ανάγκη
Μέρος της εφαρμογής του ΣΕΠ είναι η διενέργεια αυτοαξιολογήσεων από τους μαθητές προκειμένου να αντληθούν περισσότερες πληροφορίες για την προσωπικότητα τους ώστε να να βοηθηθούν στην επιλογή του καταλληλότερου για αυτούς επαγγέλματος. Αυτά υλοποιούνται είτε μέσω γραπτών αυτοαξιολογήσεων είτε με ηλεκτρονικά ερωτηματολόγια. Θεωρούμε ότι η υλοποίηση των τεστ αυτοαξιολόγησης μέσω ενός εικονικου βοηθού μπορεί να βοηθήσει συμπληρωματικά το έργο ενός Υπευθύνου ΣΕΠ καθώς κάνει την διαδικασία περισσότερο ελκυστική στον μαθητή ενώ παράλληλα μπορεί να εξαχθούν οι καταάλληλες συμβουλές μέσω ενός μοντέλου τεχνητής νοημοσύνης
### Προτεινόμενη λύση
Σκοπός μας είναι η δημιουργία ενός εικονικού βοηθού ΣΕΠ με εργαλεία ανοικτού λογισμικού. Για τον σκοπό αυτό θα χρειαστεί να υλοποιήσουμε μία εφαρμογή για κινητά (android) που θα λειτουργεί ώς frontend για τον χρήστη. Αυτή η εφαρμογή θα υλοποιηθεί με το app inventor. Επιπλέον θα υλοποιηθεί και το μοντέλο τεχνητής νοημοσύνης μέσω του RASA, που είναι ένα περιβάλλον ανοικτού κώδικα ανάπτυξης εικονικών βοηθών. 
### Κόστος
Ενδεχομένως για την εκπαίδευση του μοντέλου καθώς και για την λειτουργία του server που θα παρέχει υπηρεσίες ερωτοαπαντήσεων θα πρέπει να νοικιαστεί χώρος φιλοξενίας σε εταιρίες εξιδικευμένες για αυτό τον σκοπό. Το ποσό ετησίως μπορεί να ανέλθει στα 200 ευρώ. Εναλλακτικά θα μπορούσε να υλοποιηθεί η λύση χρήσης open hardware για την εκπαίδευση του μοντέλου, άλλα εξαρτάται από τις τελικές απαιτήσεις σε επεξεργαστική ισχύ.
Ιστορικό
Μετά από έρευνα και μελέτη των μεγάλων γλωσσικών μοντέλων (LLMs) προτιμήθηκαν αυτά τα μοντέλα έναντι της αρχικής επιλογής χρησιμοποίησης της πλατφόρμας RASA. 

## Εργαλεία
### https://github.com/oobabooga/text-generation-webui
Οδηγός χρήσης (linux):
Αρχικά αντιγράφουμε μέσω git clone τον κώδικα, και "τρέχουμε" το πρόγραμμα δίνοντας από το τερματικό την εντολή ./start_linux.sh --api. Μετά την εκτέλεση θα μας δοθεί η δυνατότητα διαχείρισης του μοντέλου, μέσω ενός web περιβάλλοντος που θα έχουμε πρόσβαση από το τοπικό περιβάλλον του Η/Υ στην διεύθυνση http://127.0.0.1:7860. Παράλληλα μέσω της παραμέτρου api μπορούμε να δώσουμε την δυνατότητα κλήσεων μέσω συμβατού προτύπου openai api στην αντίστοιχη διεύθυνση 127.0.0.1:5000
Με την χρήση του τοπικού περιβάλλοντος μπορούμε να ρυθμίσουμε το μοντέλο μας έτσι ώστε να το "φορτώσουμε" για να χρησιμοποιηθεί στις ανταπαντήσεις.
Το μοντέλο που επιλέχθηκε να χρησιμοποιηθεί για τις ανάγκες μας, είναι το meltemi. Το meltemi αναπτύχθηκε από το Ινστιτούτο Γλώσσας και επεξεργασίας του λόγου, και βασίζεται στο ανοικτό μοντέλο mistral. Επιλέχθηκε γιατί το μοντέλο έχει μετεκπαιδευτεί στην ελληνική γλώσσα. Σχετικά, https://opengov.ellak.gr/2024/03/29/meltemi-ena-elliniko-llm/, https://huggingface.co/ilsp.

Στην περίπτωση μας χρησιμοποιήθηκε η έκδοση https://huggingface.co/ilsp/Meltemi-7B-Instruct-v1-GGUF. Επιλέχθηκε το συγκεκριμένο λόγω περιορισμών στο υλικό.Ο λόγος είναι ότι για την φόρτωση και λειτουργία ενός μοντέλου, απαιτείται ισχυρή επεξεργαστική ισχύ με την χρήση μονάδων καρτών γραφικών που δεν διαθέτει ο μέσος χρήστης. Για την πρόσβαση σε τέτοιες υπηρεσίες υπάρχει αντίστοιχο κόστος. Για αυτή την περίπτωση έχει αναπτυχθεί η βιβλιοθήκη λογισμικου GGUF που παρέχει την δυνατότητα λειτουργίας ενός μοντέλου ακόμη και σε απλές CPU, θυσιάζοντας εν μέρει την αποτελεσματικότητα του μοντέλου. Μετά από δοκιμές επιλέχθηκε η έκδοση meltemi-instruct-v1_q5_K_M.bin γιατί το πιο απλό meltemi-instruct-v1_q3_K_M.bin δεν απέδιδε καλά.
Το μοντέλο φορτώθηκε και αρχικά δοκιμάστηκε μέσω του περιβάλλοντος web-gui φώτο, ενώ στην συνέχεια χρησιμοποιήθηκε το api μέσω της εφαρμογής του app inventor. Μέσω αρκετών πειραματισμών καταλήξαμε στο καταλληλότερη ρύθμιση βάση και των δυνατοτήτων. Το αποτέλεσμα κρίνεται σχετικά ικανοποιητικό για πειραματική χρήση. Τα κύρια προβλήματα που υπάρχουν μέχρι στιγμής είναι τα εξής:
- αργή ανταπόκριση
- μη ολοκλήρωση μίας συνεδρίας μέχρι την επιλογή επαγγέλματος
- κάποιες φορές οι απαντήσεις δεν επιστρέφουν, (χάνονται;)
- άσχετες απαντήσεις σε σχέση με το θέμα
- απαντήσεις στα αγγλικά
### app inventor
Το app inventor είναι ένα προγραμματιστικο περιβάλλον με τουβλάκια (blocks) που οδηγούν στην δημιουργία εφαρμογών για κινητά android. Με την χρήση του δημιουργήσαμε το πρόγραμμα πελάτη μέσω του οποίου επικοινωνεί ο χρήστης με το μοντέλο. Δίνεται η δυνατότητα επικοινωνίας και με φωνητική ομιλία χρησιμοποιώντας αντίστοιχη υπηρεσία της Google από τα κινητά. Για την υλοποίηση του χρησιμοποιήσαμε διάφορους components. Η πιο μεγάλη πρόκληση ήταν η επικοινωνία με το μοντέλο μέσω api κλήσεων, που προϋπέθετε την χρήση δεδομένων json. Με την βοήθεια του οδηγού https://ai2.appinventor.mit.edu/reference/blocks/dictionaries.html και τις αντίστοιχες οδηγίες του openai https://platform.openai.com/docs/api-reference/chat μπορέσαμε να πετύχουμε την επικοινωνία μεταξύ προγράμματος πελάτη και μοντέλου.

## Υλοποίηση
Η υλοποίηση του μοντέλου έγινε σε ένα laptop με χαρακτηριστικά i5-7200U+4 16GB RAM. Αφού ενεργοποιήθηκε το webui και ρυθμίστηκε το μοντέλο, χρησιμοποιήσαμε ένα πρόγραμμα tunnelling το localtunnel https://github.com/localtunnel/localtunnel, μέσω του οποίου ήταν δυνατή η προσβαση της εφαρμογής app inventor. Αφού δοκιμάστηκε το app inventor μέσω το πρόγραμμα προσομείωσης του κινητού. Όταν ολοκληρώθηκε η διαδικασία ανάπτυξης παράχθηκε το αντίστοιχο  


 
- https://huggingface.co/ilsp/Meltemi-7B-Instruct-v1-GGUF

https://dide-new.fth.sch.gr/sep/?page_id=40

https://www.esos.gr/arthra/76688/odigies-gia-tin-ylopoiisi-toy-sholikoy-epaggelmatikoy-prosanatolismoy-tis-g-taxis

https://blogs.sch.gr/kesyplam/

https://www.minedu.gov.gr/aei-9/nomothesia-aei/298-uncategorised/2397-sep

https://www.esos.gr/arthra/76909/systima-pistopoiisis-eparkeias-prosonton-symvoylon-stadiodromiasepaggelmatikoy


