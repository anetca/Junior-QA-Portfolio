## Ukázka testovacích scénářů
Tyto testovací scénáře pro funkce **Create Joke** a **Update Joke** jsem vytvořila během kurzu podle dokumentace.

**Create Joke:** 
1. Create joke - name and text
2. Create joke - name and image
3. Create joke - name, text and image
4. Create joke - name, text and one category
5. Create joke - name, image and one category
6. Create joke - name, text, image and one category
7. Create joke - user clicks on cancel button during joke creation
8. Create joke - text nor image are provided
9. Create joke - character limit for name and text
10. Create joke - category selection limit

**Update Joke:** 
1. Update joke - change name
2. Update joke - change text
3. Update joke - change image
4. Update joke - delete text, add image
5. Update joke - delete image, change text
6. Update joke - leaving text and image fields empty should show a warning message
7. Update joke - clicking on the cancel button during joke update should show a warning message
8. Update joke - updating a joke you didn’t create should not be possible
