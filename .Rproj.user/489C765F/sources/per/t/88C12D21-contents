library(ggfortify)
Stresslevel <- read.csv("Stesslevel.csv", sep = ",")
Stresslevel <- Stresslevel[,]
pca_res <- prcomp(Stresslevel, scale = TRUE)

autoplot(pca_res, data =Stresslevel, colour = "Cases")