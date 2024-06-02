# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Fitting Vector Generalized Linear and Additive Models Use VGAM With (In) R Software
install.packages("VGAM")
library("VGAM")
VGAM = read.csv("https://raw.githubusercontent.com/timbulwidodostp/VGAM/main/VGAM/VGAM.csv",sep = ";")
# Estimate Fitting Vector Generalized Linear and Additive Models Use VGAM With (In) R Software
VGAM_1 <- vgam(cbind(normal, mild, severe) ~ s(let), cumulative(parallel = TRUE), data = VGAM, trace = TRUE)
summary(VGAM_1)
VGAM_2 <- vglm(cbind(normal, mild, severe) ~ let, multinomial, VGAM)
summary(VGAM_2)
VGAM_3 <- vglm(cbind(normal, mild, severe) ~ let, propodds, VGAM)
summary(VGAM_2)
# Fitting Vector Generalized Linear and Additive Models Use VGAM With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished