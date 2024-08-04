# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Regression Semi-Parametric models for Interval Censored Data Use ic_sp (icenReg) With (In) R Software
install.packages("icenReg")
library("icenReg")
icenReg = read.csv("https://raw.githubusercontent.com/timbulwidodostp/icenReg/main/icenReg/icenReg.csv",sep = ";")
# Estimation Regression Semi-Parametric models for Interval Censored Data Use ic_sp (icenReg) With (In) R Software
icenReg_1 <- ic_sp(Surv(l, u, type = 'interval2') ~ x1 + x2, data = icenReg)	
summary(icenReg_1)		
icenReg_2 <- ic_sp(Surv(l, u, type = 'interval2') ~ x1 + x2, data = icenReg, model = 'po')
summary(icenReg_2)
# Regression Semi-Parametric models for Interval Censored Data Use ic_sp (icenReg) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished