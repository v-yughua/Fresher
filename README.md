# Fresher
 public GetActivityInfoResult GetLotteryResult(string OpenId, int activityId)
        {
            GetActivityInfoResult result = null;

            switch (activityId)
            {
                case 1:
                    result = MilkingLottery(OpenId, activityId);
                    break;
                case 2:
                    result = RedMoneyForNewRegisterLottery(OpenId, activityId);
                    break;
                case 4:
                    result = SignInLottery(OpenId, activityId);
                    break;
                case 5:
                    result = ZeroPayShoppingLottery(OpenId, activityId);
                    break;
                default:
                    break;
            }

            return result;
        }
