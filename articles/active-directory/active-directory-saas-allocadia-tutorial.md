---
title: 'Tutorial: Azure Active Directory integration with Allocadia | Microsoft Docs'
description: Learn how to configure single sign-on between Azure Active Directory and Allocadia.
services: active-directory
documentationcenter: ''
author: jeevansd
manager: femila
editor: ''

ms.assetid: c415fc55-6dc1-49f2-a8a2-2fc6e3790d65
ms.service: active-directory
ms.workload: identity
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: article
ms.date: 3/10/2017
ms.author: jeedes

---
# Tutorial: Azure Active Directory integration with Allocadia
In this tutorial, you learn how to integrate Allocadia with Azure Active Directory (Azure AD).

Integrating Allocadia with Azure AD provides you with the following benefits:

* You can control in Azure AD who has access to Allocadia
* You can enable your users to automatically sign in to Allocadia using single sign-on (SSO) with their Azure AD accounts
* You can manage your accounts in one central location - the Azure classic portal

If you want to know more details about SaaS app integration with Azure AD, see [What is application access and single sign-on with Azure Active Directory](active-directory-appssoaccess-whatis.md).

## Prerequisites
To configure Azure AD integration with Allocadia, you need the following items:

* An Azure AD subscription
* A Allocadia SSO enabled subscription

>[!NOTE]
>To test the steps in this tutorial, we do not recommend using a production environment. 
> 

To test the steps in this tutorial, you should follow these recommendations:

* You should not use your production environment, unless this is necessary.
* If you don't have an Azure AD trial environment, you can get a [one-month trial](https://azure.microsoft.com/pricing/free-trial/).

## Scenario Description
In this tutorial, you test Azure AD SSO in a test environment. 

The scenario outlined in this tutorial consists of two main building blocks:

1. Adding Allocadia from the gallery
2. Configuring and testing Azure AD SSO

## Add Allocadia from the gallery
To configure the integration of Allocadia into Azure AD, you need to add Allocadia from the gallery to your list of managed SaaS apps.

**To add Allocadia from the gallery, perform the following steps:**

1. In the **Azure classic portal**, on the left navigation pane, click **Active Directory**. 
   
    ![Active Directory][1]

2. From the **Directory** list, select the directory for which you want to enable directory integration.

3. To open the applications view, in the directory view, click **Applications** in the top menu.
   
    ![Applications][2]

4. Click **Add** at the bottom of the page.
   
    ![Applications][3]

5. On the **What do you want to do** dialog, click **Add an application from the gallery**.
   
    ![Applications][4]

6. In the search box, type **Allocadia**.
   
    ![Creating an Azure AD test user](./media/active-directory-saas-allocadia-tutorial/tutorial_allocadia_01.png)

7. In the results pane, select **Allocadia**, and then click **Complete** to add the application.
   
    ![Creating an Azure AD test user](./media/active-directory-saas-allocadia-tutorial/tutorial_allocadia_06.png)

## Configure and test Azure AD single sign-on
In this section, you configure and test Azure AD SSO with Allocadia based on a test user called "Britta Simon".

For SSO to work, Azure AD needs to know what the counterpart user in Allocadia is to a user in Azure AD. In other words, a link relationship between an Azure AD user and the related user in Allocadia needs to be established.

This link relationship is established by assigning the value of the **user name** in Azure AD as the value of the **Username** in Allocadia.

To configure and test Azure AD SSO with Allocadia, you need to complete the following building blocks:

1. **[Configuring Azure AD single sign-on](#configuring-azure-ad-single-single-sign-on)** - to enable your users to use this feature.
2. **[Creating an Azure AD test user](#creating-an-azure-ad-test-user)** - to test Azure AD single sign-on with Britta Simon.
3. **[Creating an Allocadia test user](#creating-an-allocadia-test-user)** - to have a counterpart of Britta Simon in Allocadia that is linked to the Azure AD representation of her.
4. **[Assigning the Azure AD test user](#assigning-the-azure-ad-test-user)** - to enable Britta Simon to use Azure AD single sign-on.
5. **[Testing single sign-on](#testing-single-sign-on)** - to verify whether the configuration works.

### Configure Azure AD single sign-on
In this section, you enable Azure AD SSO in the classic portal and configure SSO in your Allocadia application.

Allocadia application expects the SAML assertions in a specific format. Please configure the following claims for this application. You can manage the values of these attributes from the **"Atrribute"** tab of the application. The following screenshot shows an example for this. 

![Configure Single Sign-On](./media/active-directory-saas-allocadia-tutorial/tutorial_allocadia_07.png) 

**To configure Azure AD single sign-on with Hightail, perform the following steps:**

1. In the Azure classic portal, on the **Allocadia** application integration page, in the menu on the top, click **Attributes**.
   
    ![Configure Single Sign-On](./media/active-directory-saas-allocadia-tutorial/tutorial_general_80.png) 

2. On the **SAML token attributes** dialog, for each row shown in the table below, perform the following steps:
   
    | Attribute Name | Attribute Value |
    | --- | --- |
    | firstname |user.givenname |
    | lastname |user.surname |
    | email |user.mail |

  1. Click **add user attribute** to open the **Add User Attribure** dialog.

    ![Configure Single Sign-On](./media/active-directory-saas-allocadia-tutorial/tutorial_general_81.png) 
  2. In the **Attrubute Name** textbox, type the attribute name shown for that row.
  3. From the **Attribute Value** list, selsect the attribute value shown for that row.
  4. Click **Complete**.    
 
3. In the menu on the top, click **Quick Start**.
   
    ![Configure Single Sign-On](./media/active-directory-saas-allocadia-tutorial/tutorial_general_83.png)  

4. On the **How would you like users to sign on to Allocadia** page, select **Azure AD Single Sign-On**, and then click **Next**.
   
    ![Configure Single Sign-On](./media/active-directory-saas-allocadia-tutorial/tutorial_allocadia_03.png) 

5. On the **Configure App Settings** dialog page, perform the following steps:.
   
    ![Configure Single Sign-On](./media/active-directory-saas-allocadia-tutorial/tutorial_allocadia_04.png)  
  1. In the IDENTIFER box type the URL in the following pattern: For test environment use the URL as **"https://na2standby.allocadia.com"** and for production environment use **"https://na2.allocadia.com"**.
  2. In the Reply URL type the URL in the following pattern: For test environment use the URL pattern as  **"https://na2standby.allocadia.com/allocadia/saml/SSO"** and for production environment use **"https://na2.allocadia.com/allocadia/saml/SSO"**

6. On the **Configure single sign-on at Allocadia** page, perform the following steps:
   
    ![Configure Single Sign-On](./media/active-directory-saas-allocadia-tutorial/tutorial_allocadia_05.png) 
  1. Click **Download metadata**, and then save the file on your computer.
  2. Click **Next**.

7. To get SSO configured for your application, contact [Allocadia Support](mailTo:support@allocadia.com) team and they will assist to configure SSO. Please note that you have to send email and attach downloaded metadata file to configure SSO on the Allocadia side.
   
   >[!NOTE]
   >Please make sure that Allocadia team set the Identifier value in the test environment as **"https://na2standby.allocadia.com"** and for production environment, it should be: **"https://na2.allocadia.com"**
   >  

8. In the classic portal, select the single sign-on configuration confirmation, and then click **Next**.
   
    ![Azure AD Single Sign-On][10]

9. On the **Single sign-on confirmation** page, click **Complete**.  
   
    ![Azure AD Single Sign-On][11]

### CreatE an Azure AD test user
In this section, you create a test user in the classic portal called Britta Simon.

* In the Users list, select **Britta Simon**.

![Create Azure AD User][20]

**To create a test user in Azure AD, perform the following steps:**

1. In the **Azure classic portal**, on the left navigation pane, click **Active Directory**.
   
    ![Creating an Azure AD test user](./media/active-directory-saas-allocadia-tutorial/create_aaduser_09.png) 

2. From the **Directory** list, select the directory for which you want to enable directory integration.

3. To display the list of users, in the menu on the top, click **Users**.
   
    ![Creating an Azure AD test user](./media/active-directory-saas-allocadia-tutorial/create_aaduser_03.png) 

4. To open the **Add User** dialog, in the toolbar on the bottom, click **Add User**.
   
    ![Creating an Azure AD test user](./media/active-directory-saas-allocadia-tutorial/create_aaduser_04.png) 

5. On the **Tell us about this user** dialog page, perform the following steps:
   
    ![Creating an Azure AD test user](./media/active-directory-saas-allocadia-tutorial/create_aaduser_05.png) 
 1. As Type Of User, select New user in your organization.   
 2. In the User Name **textbox**, type **BrittaSimon**. 
 3. Click **Next**.

6. On the **User Profile** dialog page, perform the following steps:
   
    ![Creating an Azure AD test user](./media/active-directory-saas-allocadia-tutorial/create_aaduser_06.png)  
 1. In the **First Name** textbox, type **Britta**.    
 2. In the **Last Name** textbox, type, **Simon**. 
 3. In the **Display Name** textbox, type **Britta Simon**. 
 4. In the **Role** list, select **User**. 
 5. Click **Next**.

7. On the **Get temporary password** dialog page, click **create**.
   
    ![Creating an Azure AD test user](./media/active-directory-saas-allocadia-tutorial/create_aaduser_07.png) 

8. On the **Get temporary password** dialog page, perform the following steps:
   
    ![Creating an Azure AD test user](./media/active-directory-saas-allocadia-tutorial/create_aaduser_08.png)  
 1. Write down the value of the **New Password**.  
 2. Click **Complete**.   

### CreatE an Allocadia test user
In this section, you create a user called Britta Simon in Allocadia. Allocadia application support just in time user provisioning. If you have configured the claims as stated above in **[Configuring Azure AD Single Sign-On](#configuring-azure-ad-single-single-sign-on)** section then it will provision the users in the application. 

>[!NOTE]
>If you need to create a user manually or batch of users, you need to contact the Allocadia support team. 
> 

### Assign the Azure AD test user
In this section, you enable Britta Simon to use Azure sso by granting her access to Allocadia.

![Assign User][200] 

**To assign Britta Simon to Allocadia, perform the following steps:**

1. On the classic portal, to open the applications view, in the directory view, click **Applications** in the top menu.
   
    ![Assign User][201] 

2. In the applications list, select **Allocadia**.
   
    ![Configure Single Sign-On](./media/active-directory-saas-allocadia-tutorial/tutorial_allocadia_50.png) 

3. In the menu on the top, click **Users**.
   
    ![Assign User][203] 

4. In the Users list, select **Britta Simon**.

5. In the toolbar on the bottom, click **Assign**.
   
    ![Assign User][205]

### Test Single Sign-On
In this section, you test your Azure AD sso configuration using the Access Panel.

When you click the Allocadia tile in the Access Panel, you should get automatically signed-on to your Allocadia application.

## Additional Resources
* [List of Tutorials on How to Integrate SaaS Apps with Azure Active Directory](active-directory-saas-tutorial-list.md)
* [What is application access and single sign-on with Azure Active Directory?](active-directory-appssoaccess-whatis.md)

<!--Image references-->

[1]: ./media/active-directory-saas-allocadia-tutorial/tutorial_general_01.png
[2]: ./media/active-directory-saas-allocadia-tutorial/tutorial_general_02.png
[3]: ./media/active-directory-saas-allocadia-tutorial/tutorial_general_03.png
[4]: ./media/active-directory-saas-allocadia-tutorial/tutorial_general_04.png

[6]: ./media/active-directory-saas-allocadia-tutorial/tutorial_general_05.png
[10]: ./media/active-directory-saas-allocadia-tutorial/tutorial_general_06.png
[11]: ./media/active-directory-saas-allocadia-tutorial/tutorial_general_07.png
[20]: ./media/active-directory-saas-allocadia-tutorial/tutorial_general_100.png

[200]: ./media/active-directory-saas-allocadia-tutorial/tutorial_general_200.png
[201]: ./media/active-directory-saas-allocadia-tutorial/tutorial_general_201.png
[203]: ./media/active-directory-saas-allocadia-tutorial/tutorial_general_203.png
[204]: ./media/active-directory-saas-allocadia-tutorial/tutorial_general_204.png
[205]: ./media/active-directory-saas-allocadia-tutorial/tutorial_general_205.png
