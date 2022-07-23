# MasterThesisADS
To use the pre-trained model, download the word vectors for the Dutch language from: https://fasttext.cc/docs/en/crawl-vectors.html
To get the lines through the plots, use the following code in R:

###
plot(migratie$`semantic similarity`, migratie$`voting_similarity`,
xlab = "Semantic Similarity", ylab = "Voting Similarity",
pch = 19, frame = FALSE, xlim = c(0.8,1), ylim = c(0,1))
abline(lm(migratie$`semantic similarity` ~ migratie$`voting_similarity`), lty = 2, col = "red")

plot(sexualiteit$`semantic similarity`, sexualiteit$`voting_similarity`,
xlab = "Semantic Similarity", ylab = "Voting Similarity",
pch = 19, frame = FALSE, xlim = c(0.80,1), ylim = c(0,1))
abline(lm(sexualiteit$`semantic similarity` ~ sexualiteit$`voting_similarity`), lty = 2, col = "red")

plot(religie$`semantic similarity`, religie$`voting_similarity`,
xlab = "Semantic Similarity", ylab = "Voting Similarity",
pch = 19, frame = FALSE, xlim = c(0.80,1), ylim = c(0,1))
abline(lm(religie$`semantic similarity` ~ religie$`voting_similarity`),  lty = 2, col = "red")
###

We use the imported dataset for each topic from the jupyter notebook file.
