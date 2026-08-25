# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Vuong's Non-Nested Hypothesis Test-Statistic Use vuong (pscl) With (In) R Software
install.packages("pscl")
library("pscl")
# Estimate Vuong's Non-Nested Hypothesis Test-Statistic Use vuong (pscl) With (In) R Software
vuong_ = read.csv("https://raw.githubusercontent.com/timbulwidodostp/vuong_/main/vuong_/vuong_.csv",sep = ";")
glm <- glm(art ~ ., data = vuong_, family = poisson)
zeroinfl <- zeroinfl(art ~ . | ., data = vuong_, EM = TRUE)
vuong(glm, zeroinfl)
# Vuong's Non-Nested Hypothesis Test-Statistic Use vuong (pscl) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished