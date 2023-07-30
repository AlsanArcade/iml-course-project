# iml-course-project

I train Unets for each timestep to predict the contrail mask.   
Then I stack the output mask of those and pass them to another Unet which predicts the final mask.    

The dice_val of the Stack (```val_dice = 0.611```) improved on the best performing single timestep model(t_null) (```val_dice = 0.602```)    
   
While this is only a very minor improvment, it shows that including all timesteps in the model should increases the performance
