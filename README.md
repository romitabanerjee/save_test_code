# save_test_code

Few comments:
1.	All the data cleanup is done in mysql. 
2.	“alter_accountInfo” and “alter_transactions” contain the necessary queries for data preprocessing
3.	For rule 1, I’ve assumed that any transaction amount which is fives times higher than the average(for that specific user) means a fraudulent transaction
4.	I’ve also implemented another version for rule 1, where the fraud transactions are flagged based upon the z-scores of the transaction amount.
5.	This rule is in the stored proc “rule_1_zscore” but is not used in the visual studio project.
