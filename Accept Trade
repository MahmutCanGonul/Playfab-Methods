private void AcceptTrade()
    {
        PlayFabClientAPI.AcceptTrade(new AcceptTradeRequest
        {

            AuthenticationContext = new PlayFabAuthenticationContext
            {
                PlayFabId = "USER_PLAYFABID",
                EntityToken = "USER_TOKEN",
                EntityId = "USER_ENTITYID",
                EntityType = "USER_ENTITYTYPE",
                ClientSessionTicket = "USERCLIENTSESSION"
            },
            TradeId = "TRADE_ID",
            AcceptedInventoryInstanceIds = new List<string> { "ITEM_1_ID", "ITEM_2_ID" } ,
            OfferingPlayerId= "PLAYFABID" // Playeid is Who open the trade 

        }, resultCallback => { Debug.Log("Trade is : " + resultCallback.Trade.Status); }, errorCallback => { Debug.Log(errorCallback.ErrorMessage); });

    }
