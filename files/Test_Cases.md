## Ukázka testovacích případů

Tyto testovací případy pro funkci **Create Joke** jsem vytvořila během kurzu podle dokumentace.

|   |   |
|---|---|
| Test case ID  |  JC_001 |
| Title |  **Create joke - name and text** |
| Description | Verify that the system allows a user to create a joke with name and text successfully and displays a confirmation message.|
| Preconditions |- User is logged into the system.<br>- User has access to the joke creation feature.|
| Test Steps | 1. Open the joke creation form<br>2. Fill in a valid name and valid text<br>3. Confirm the form |
| Test Data | *- Valid name length is 255 characters or fewer.<br>- Valid text length is 4000 characters or fewer.*|
| Expected Result  | The system creates the joke and displays a confirmation: The joke <joke.name> was successfully created. |

|   |   |
|---|---|
| Test case ID  |  JC_002 |
| Title | **Create joke - name and image**  |
| Description | Verify that the system allows a user to create a joke with name and image successfully and displays a confirmation message.|
| Preconditions |- User is logged into the system.<br>- User has access to the joke creation feature.|
| Test Steps |  1. Open the joke creation form<br>2. Fill in a valid name and upload an image<br>3. Confirm the form |
| Test Data | *Valid name length is 255 characters or fewer.*|
| Expected Result  |  The system creates the joke and displays a confirmation: The joke <joke.name> was successfully created. |

|   |   |
|---|---|
| Test case ID  |  JC_003 |
| Title | **Create joke - name, text and image**  |
| Description | Verify that the system allows a user to create a joke with name, text and image successfully and displays a confirmation message.|
| Preconditions |- User is logged into the system.<br>- User has access to the joke creation feature.|
| Test Steps |  1. Open the joke creation form<br>2. Fill in a valid name, valid text and upload an image<br>3. Confirm the form |
| Test Data | *- Valid name length is 255 characters or fewer.<br>- Valid text length is 4000 characters or fewer.*|
| Expected Result  |  The system creates the joke and displays a confirmation: The joke <joke.name> was successfully created. |

|   |   |
|---|---|
| Test case ID  |  JC_004 |
| Title |  **Create joke - name, text and category** |
| Description | Verify that the system allows a user to create a joke with name, text and one category successfully and displays a confirmation message.|
| Preconditions |- User is logged into the system.<br>- User has access to the joke creation feature.<br>- At least one existing category.|
| Test Steps | 1. Open the joke creation form<br>2. Fill in a valid name, valid text and select a category<br>3. Confirm the form   |
| Test Data | *- Valid name length is 255 characters or fewer.<br>- Valid text length is 4000 characters or fewer.<br>- Max. number of selected categories is 10.*|
| Expected Result  | The system creates the joke and displays a confirmation: The joke <joke.name> was successfully created. |

|   |   |
|---|---|
| Test case ID  |  JC_005 |
| Title |  **Create joke - name, image and one category** |
| Description | Verify that the system allows a user to create a joke with name, image and one category successfully and displays a confirmation message.|
| Preconditions |- User is logged into the system.<br>- User has access to the joke creation feature.<br>- At least one existing category.|
| Test Steps | 1. Open the joke creation form<br>2. Fill in a valid name, upload an image, and select a category.<br>3. Confirm the form   |
| Test Data | *- Valid name length is 255 characters or fewer.<br>- Max. number of selected categories is 10.*|
| Expected Result  | The system creates the joke and displays a confirmation: The joke <joke.name> was successfully created. |

|   |   |
|---|---|
| Test case ID  |  JC_006 |
| Title |  **Create joke - name, text, image and category** |
| Description | Verify that the system allows a user to create a joke with name, text, image and one category successfully and displays a confirmation message.|
| Preconditions |- User is logged into the system.<br>- User has access to the joke creation feature.<br>- At least one existing category.|
| Test Steps | 1. Open the joke creation form<br>2. Fill in a valid name, valid text, upload an image and select a category<br>3. Confirm the form   |
| Test Data | *- Valid name length is 255 characters or fewer.<br>- Valid text length is 4000 characters or fewer.<br>- Max. number of selected categories is 10.*|
| Expected Result  | The system creates the joke and displays a confirmation: The joke <joke.name> was successfully created. |

|   |   |
|---|---|
| Test case ID  |  JC_007 |
| Title |  **Create joke - user clicks on cancel button during joke creation** |
| Description | Verify that the system allows the user to cancel joke creation. |
| Preconditions |- User is logged into the system.<br>- User has access to the joke creation feature.|
| Test Steps | 1. Open the joke creation form<br>2. Fill in a valid name and valid text<br>3. Click on “cancel” button<br>4. Confirm the confirmation dialog |
| Test Data | *- Valid name length is 255 characters or fewer.<br>- Valid text length is 4000 characters or fewer.*|
| Expected Result  | The system should display a warning message asking if you want to proceed. Upon confirming, the system terminates the joke creation. |

|   |   |
|---|---|
| Test case ID  |  JC_008 |
| Title | **Create joke - neither text nor image are provided**|
| Description | Verify that the system does not allow a user to create a joke without providing text or image and displays a warning message.|
| Preconditions |- User is logged into the system.<br>- User has access to the joke creation feature.|
| Test Steps | 1. Open the joke creation form<br>2. Fill in a valid name, leave text and image fields empty.<br>3. Click on "create" button.|
| Test Data |*Valid name length is 255 characters or fewer*|
| Expected Result| The system should display a warning message, and the form should remain open.|

|   |   |
|---|---|
| Test case ID  |  JC_009 |
| Title |  **Create joke - character limit for name and text** |
| Description | Verify that the system does not allow a user to create a joke with invalid name and invalid text, and displays a warning message.|
| Preconditions |- User is logged into the system.<br>- User has access to the joke creation feature.|
| Test Steps | 1. Open the joke creation form<br>2. Fill in an invalid name and invalid text|
| Test Data | *- Invalid name length exceeds 255 characters.<br>- Invalid text length exceeds 4000 characters.*|
| Expected Result  | - When invalid name is entered, form should change its color and show a warning message — "The name must contain less than 255 characters."<br>- When invalid text is entered, form should change its color and show a warning message — "The joke text must contain less than 4000 characters."|
