# MSPartner – Azure Lighthouse  

This repository contains the deployment templates required to enable **Azure Lighthouse** delegation for Silicom.  

Azure Lighthouse allows Silicom to manage your subscription securely, with the appropriate level of access, while you retain full control and visibility.  

---

## 🔑 What you need to know

- You must be an **Owner** or **User Access Administrator** on the subscription in order to onboard it to Azure Lighthouse.  
- The delegation is **non-intrusive**: it does not change your resources, only grants Silicom predefined access rights.  
- At any time, you can review or remove the delegation directly from the **Azure Portal** under **Service providers**.  

---

## 🚀 Deploy to Azure

Choose the delegation level you want to grant. Clicking the button will open the Azure Portal with the pre-filled template.  

| Name | Description | Deploy |
|------|-------------|--------|
| **Silicom CSP support – Light** | Grants limited access to the subscription (baseline permissions). Can be escalated to **Reader** if needed. | [![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSilicomGroup%2FMSPartner-AzureLighthouse%2Frefs%2Fheads%2Fmain%2Flight.json){:target="_blank"} |
| **Silicom CSP support – Reader** | Grants **Reader** access to the subscription. Can be escalated to **Contributor** if needed. | [![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSilicomGroup%2FMSPartner-AzureLighthouse%2Frefs%2Fheads%2Fmain%2Freader.json){:target="_blank"} |

---

## 📖 Deployment steps

1. Click the **Deploy to Azure** button for the desired access level.  
2. The Azure Portal will open and load the delegation template.  
3. Select the **subscription** you want to onboard.  
4. Confirm the details and click **Review + Create** → **Create**.  
5. Wait for the deployment to complete (this usually takes less than a minute).  

---

## 🔍 Verification

After deployment:  
1. In the Azure Portal, go to **Azure Lighthouse** → **Service providers**.  
2. You should see **Silicom** listed with the corresponding role(s).  
3. From this blade, you can review or remove the delegation at any time.  

---

## ❓ Need help?

If you encounter issues or have questions about this process, please contact **Silicom support** at:  
📧 support@silicom.ch
