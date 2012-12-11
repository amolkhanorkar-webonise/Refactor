public class RajamantriChorShipahi extends Activity {
    	
  @Override
  protected void onPostResume() {
    super.onPostResume();
  }

  @Override
  public boolean onKeyDown(int key_code, KeyEvent event) {
    AlertDialog dialog = new AlertDialog.Builder(this).create();
    dialog.setTitle("Exit from game!");
    dialog.setMessage("Are you sure you want to exit the game?");
    dialog.setButton("Exit", new DialogInterface.onClickListener() {
			
  public void onClick(DialogInterface dialog, int which) {
    finish();				
			}
  });
  dialog.setButton("Cancel", new DialogInterface.onClickListener() {
			
  public void onClick(DialogInterface dialog, int which) {
				
    dialog.dismiss();
    }
  });
  dialog.show();
  return super.onKeyDown(key_code, event);
  }

  @Override
  public void onLowMemory() {
    AlertDialog dialog = new AlertDialog.Builder(this).create();
    dialog.setTitle("Low memory!");
    dialog.setMessage("Too many apps open, kindly close some other apps and try again!");
    dialog.setButton("Exit", new DialogInterface.onClickListener() {
			
  public void onClick(DialogInterface dialog, int which) {
				
    finish();
    }
  });
		
  dialog.show();

  super.onLowMemory();
  }

  @Override
  protected void onPause() {
		
    super.onPause();
  }

  String[] solutionArray = { "RAJA", "MANTRI", "CHOR", "SIPAHI"};
  String[] playersArray = {"player_one", "player_two", "player_three", "player_four"};
    static String player_one_name = "" ;
    static String player_two_name = "";
    static String player_three_name = "";
    static String player_four_name = "";
    static String player_one_role = "";
    static String player_two_role = "";
    static String player_three_role = "";
    static String player_four_role = "";
    static boolean guess = false;
    static String player_one = "";
    static String player_two = "";
    static String player_three = "";
    static String player_four = "";
    static int i=0,j=0,k=0,l=0;
    static int p_one_score = 0;
    static int p_two_score = 0;
    static int p_three_score = 0;
    static int p_four_score = 0;
    int count = 0;
	
    Button btnRajaMantri;
    Button btnHelp;
    ImageView btn9;
    Button btnPlay;
    static Button btnPod1;
    static Button btnPod2;
    static Button btnPod3;
    static Button btnPod4;
    	
    
    EditText editTxtplayer_one;
    EditText editTxtplayer_two;
    EditText editTxtplayer_three;
    EditText editTxtplayer_four;
    TextView lblplayer_one;
    TextView lblplayer_two;
    TextView lblplayer_three;
    TextView lblplayer_four;
    static TextView txtTurn;
    static TextView txtplayer_one;
    static TextView txtplayer_two;
    static TextView txtplayer_three;
    static TextView txtplayer_four;
    Bundle savedInstanceState2;
    Button btnMainMenu;	
    
    String nextTurn = "";
		
    public void onRestart(){
    	
    super.onRestart(); 	
    	
    }
    
    public void onResume(){
    	
    super.onResume();
    	  	
    	
    }

    public void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.welcome);
      
    i = 0;        j = 0;        k = 0;        l = 0;
    btnHelp = (Button)findViewById(R.id.btnHelp);
    btnHelp.setOnClickListener(new onClickListener() {
			
  public void onClick(View v) {
    setContentView(R.layout.help);		 // Create the adView
    AdView adView = new AdView(RajaMantri.this, AdSize.BANNER, "a14e156523d01de");
			    // Lookup your LinearLayout assuming it’s been given
			    // the attribute android:id="@+id/mainLayout"
    LinearLayout layout = (LinearLayout)findViewById(R.id.mainLayoutHelp);
			    // Add the adView to it
    layout.addView(adView);
			    // Initiate a generic request to load it with an ad
    adView.loadAd(new AdRequest());
    TextView txtHelp = (TextView)findViewById(R.id.txtHelp);
    String text = "Welcome to nostalgia! This is the paper free version of Raja Mantri Chor Sipahi.\n\nThe game involves bluffing with facial expressions and good guessing. This is a very popular childhood game in India played among kids often during their long summer vacations.\n\nThe game has 4 paper chits with Chor (thief), Sipahi (police), Raja (king) and Mantri (minister). The chits are folded at the start of the game and one of the 4 players will press SHUFFLE each one of the four players is supposed to secretly (by taking the phone and not letting the others see it)pick one chit by clicking on it, the player then clicks on the chit again to fold it back. All the players will then secretly open their chits and read what they have got. \n\nThe player who gets the chit with Raja written on it will say MERA MANTRI KAUN? (Who is my minister?). The player who got the chit with Mantri will say MEIN! (Me), The player with Raja will then say CHOR SIPAHI KA PATA LAGAO (find out who is the theif and who is the soldier). The player with Mantri will then guess who is the Chor (Thief), if he is wrong then his points are deducted and if he is correct he gets more points and the points from the player who got Chor (Thief) are deducted.\n\nIf the guess is correct the player with Chor is wrapped on his wrist by the Mantri, and if the Mantri is wrong then the Chor gets to hit his wrist.";
    txtHelp.setText(text);
    Button btnBack = (Button)findViewById(R.id.btnMainMenuHelp);
    btnBack.setOnClickListener(new onClickListener() {
					
  public void onClick(View v) {					
    Intent i = new Intent(RajaMantri.this, RajaMantri.class);
    RajaMantri.this.startActivity(i);
    finish();
				
    }
    });
    }
  });
    btnRajaMantri = (Button) findViewById(R.id.btnRajaMantri);
    btnRajaMantri.setOnClickListener(new onClickListener() {
        	
 public void onClick(View v) {
 			// TODO Auto-generated method stub
   setContentView(R.layout.rmcsp);	
 		 // Create the adView
   AdView adView = new AdView(RajaMantri.this, AdSize.BANNER, "a14e156523d01de");
	    // Lookup your LinearLayout assuming it’s been given
	    // the attribute android:id="@+id/mainLayout"
   LinearLayout layout = (LinearLayout)findViewById(R.id.mainLayoutPlayer);
	    // Add the adView to it
   layout.addView(adView);
	    // Initiate a generic request to load it with an ad
   adView.loadAd(new AdRequest());
	    
   editTxtplayer_one = (EditText) findViewById(R.id.editTxtplayer_one);
   editTxtplayer_two = (EditText)findViewById(R.id.editTxtplayer_two);
   editTxtplayer_three = (EditText)findViewById(R.id.editTxtplayer_three);
   editTxtplayer_four = (EditText)findViewById(R.id.editTxtplayer_four);
 		
   lblplayer_one = (TextView) findViewById(R.id.lblplayer_one);
   lblplayer_two = (TextView) findViewById(R.id.lblplayer_two);
   lblplayer_three = (TextView) findViewById(R.id.lblplayer_three);
   lblplayer_four = (TextView) findViewById(R.id.lblplayer_four);
 		
   Display display = getWindowManager().getDefaultDisplay(); 
   int width = display.getWidth();
   int height = display.getHeight();
 		
 		
 		
   lblplayer_one.setGravity(Gravity.CENTER_HORIZONTAL);
   lblplayer_two.setGravity(Gravity.CENTER_HORIZONTAL);
   lblplayer_three.setGravity(Gravity.CENTER_HORIZONTAL);
   lblplayer_four.setGravity(Gravity.CENTER_HORIZONTAL);
 	 		
   Log.v("AkandBakar", "Playernames:" + player_one_name);
   Log.v("AkandBakar", "Playernames:" + player_two_name);
   Log.v("AkandBakar", "Playernames:" + player_three_name);
   Log.v("AkandBakar", "Playernames:" + player_four_name);
 		
   btnMainMenu = (Button) findViewById(R.id.btnMainMenu);
   btnMainMenu.setOnClickListener(new onClickListener() {
			
  public void onClick(View v) {
    Intent i = new Intent(RajaMantri.this, RajaMantri.class);
    RajaMantri.this.startActivity(i);
    finish();
    }
  });
 		
    btnSignin = (Button) findViewById(R.id.btnsignin);
    btnSignin.setOnClickListener(new onClickListener() {
			
  public void onClick(View v) {					
    player_one_name = editTxtplayer_one.getText().toString();
    player_two_name = editTxtplayer_two.getText().toString();
    player_three_name = editTxtplayer_three.getText().toString();
    player_four_name = editTxtplayer_four.getText().toString();
		 		 		
    if(player_one_name.equals("")||player_two_name.equals("")||player_three_name.equals("")||player_four_name.equals("")){
					
    Toast toast = Toast.makeText(getBaseContext(), "Enter player names!", 8000);
    toast.show();
					
  }else{
    setContentView(R.layout.rmcsgnew);	
					 // Create the adView
    AdView adView = new AdView(RajaMantri.this, AdSize.BANNER, "a14e156523d01de");
				    // Lookup your LinearLayout assuming it’s been given
				    // the attribute android:id="@+id/mainLayout"
    LinearLayout layout = (LinearLayout)findViewById(R.id.mainLayout);
				    // Add the adView to it
    layout.addView(adView);
				    // Initiate a generic request to load it with an ad
    adView.loadAd(new AdRequest());

    txtTurn = (TextView)findViewById(R.id.txtTurn);
    txtTurn.setText("Click on SHUFFLE!");
    playersArray[0] = player_one_name;
    playersArray[1] = player_two_name;
    playersArray[2] = player_three_name;
    playersArray[3] = player_four_name; 			
    txtplayer_one = (TextView) findViewById(R.id.txtplayer_one);
    txtplayer_one.setText("1."+player_one_name + " [" + p_one_score + "]");
					
    txtplayer_two = (TextView) findViewById(R.id.txtplayer_two);
    txtplayer_two.setText("2."+player_two_name+ " [" + p_two_score + "]");
					
    txtplayer_three = (TextView) findViewById(R.id.txtplayer_three);
    txtplayer_three.setText("3."+player_three_name+ " [" + p_three_score + "]");
					
    txtplayer_four = (TextView) findViewById(R.id.txtplayer_four);
    txtplayer_four.setText("4."+player_four_name+ " [" + p_four_score + "]");
					
    btnPlay = (Button) findViewById(R.id.btnPlay);
				
    btnPlay.setOnClickListener(new onClickListener() {
		 			
  public void onClick(View v) {
		 			
    if(btnPlay.getText().equals("SHUFFLE")){
		 				
    RajaMantri.this.shuffle();
		 					
    }else{
		 							 					
    RajaMantri.this.makeGuess();
										
    Log.v("RajaMantri", "########## Player Name:" + player_one_name +" Role:" + player_one_role);
    Log.v("RajaMantri", "########## Player Name:" + player_two_name +" Role:" + player_two_role);
    Log.v("RajaMantri", "########## Player Name:" + player_three_name +" Role:" + player_three_role);
    Log.v("RajaMantri", "########## Player Name:" + player_four_name +" Role:" + player_four_role);
   }
  }
  });
  }
  }
		     
  });
  }
		
  });
 		 
       
  }
    
    
  public void makeGuess(){
    	
    btnPlay.setText("SHUFFLE");
    count = 0;
    btnPlay.setText("SHUFFLE");
			
    btnPod1.setClickable(true);
    btnPod2.setClickable(true);
			btnPod3.setClickable(true);
			btnPod4.setClickable(true);
			
		if(player_one.equals("RAJA")){
			
			btnPod1.setText("RAJA");
			btnPod1.setBackgroundResource(R.drawable.podopen);
			btnPod1.setClickable(false);
		}
		if(player_two.equals("RAJA")){
			
			btnPod2.setText("RAJA");
			btnPod2.setBackgroundResource(R.drawable.podopen);
			btnPod2.setClickable(false);
		}
		if(player_three.equals("RAJA")){

			btnPod3.setText("RAJA");
			btnPod3.setBackgroundResource(R.drawable.podopen);
			btnPod3.setClickable(false);
		}
		if(player_four.equals("RAJA")){

			btnPod4.setText("RAJA");
			btnPod4.setBackgroundResource(R.drawable.podopen);
			btnPod4.setClickable(false);
		}

		if(player_one.equals("MANTRI")){
			
			btnPod1.setText("MANTRI");
			btnPod1.setBackgroundResource(R.drawable.podopen);
			btnPod1.setClickable(false);
		}
		if(player_two.equals("MANTRI")){
			
			btnPod2.setText("MANTRI");
			btnPod2.setBackgroundResource(R.drawable.podopen);
			btnPod2.setClickable(false);
		}
		if(player_three.equals("MANTRI")){

			btnPod3.setText("MANTRI");
			btnPod3.setBackgroundResource(R.drawable.podopen);
			btnPod3.setClickable(false);
		}
		if(player_four.equals("MANTRI")){

			btnPod4.setText("MANTRI");
			btnPod4.setBackgroundResource(R.drawable.podopen);
			btnPod4.setClickable(false);
			
		}
		
		if(player_one_role.equals("MANTRI")){
			txtTurn.setText(player_one_name + " will find the CHOR!");
		}
		if(player_two_role.equals("MANTRI")){
			txtTurn.setText(player_two_name + " will find the CHOR!");
		}
		if(player_three_role.equals("MANTRI")){
			txtTurn.setText(player_three_name + " will find the CHOR!");
		}
		if(player_four_role.equals("MANTRI")){
			txtTurn.setText(player_four_name + " will find the CHOR!");
		}
		
		Log.v("AkhandBakar","#########" + btnPod1.getText());
		
		if(btnPod1.getText().equals("")){
			
			btnPod1.setOnClickListener(new onClickListener() {
				
			
				public void onClick(View v) {
					// TODO Auto-generated method stub
					Log.v("AkhandBakar","#########" + player_one);
					if(player_one.equals("CHOR")){
					
						RajaMantri.guess = true;
						btnPod1.setBackgroundResource(R.drawable.podopen);
						btnPod1.setText("CHOR");
						
					}else{
						
						RajaMantri.guess = false;
						btnPod1.setBackgroundResource(R.drawable.podopen);
						btnPod1.setText("SIPAHI");
					}
					btnPod1.setClickable(false);
					btnPod2.setClickable(false);
					btnPod3.setClickable(false);
					btnPod4.setClickable(false);
					updateScore();
				}
			});
		}	
		
		
		Log.v("AkhandBakar","#########" + btnPod2.getText());
		if(btnPod2.getText().equals("")){
			
			btnPod2.setOnClickListener(new onClickListener() {
				
				public void onClick(View v) {
					
					Log.v("AkhandBakar","#########" + player_two);
					if(player_two.equals("CHOR")){
					
						RajaMantri.guess = true;
						btnPod2.setBackgroundResource(R.drawable.podopen);
						btnPod2.setText("CHOR");
					}else{
						
						RajaMantri.guess = false;
						btnPod2.setBackgroundResource(R.drawable.podopen);
						btnPod2.setText("SIPAHI");
						
					}
					btnPod1.setClickable(false);
					btnPod2.setClickable(false);
					btnPod3.setClickable(false);
					btnPod4.setClickable(false);
					updateScore();
				}
			});
		}	
    	
		Log.v("AkhandBakar","#########" + btnPod3.getText());
		if(btnPod3.getText().equals("")){
			
			btnPod3.setOnClickListener(new onClickListener() {
				
				
				public void onClick(View v) {
					
					Log.v("AkhandBakar","#########" + player_three);
					if(player_three.equals("CHOR")){
					
						RajaMantri.guess = true;
						btnPod3.setBackgroundResource(R.drawable.podopen);
						btnPod3.setText("CHOR");
					}else{
						
						RajaMantri.guess = false;
						btnPod3.setBackgroundResource(R.drawable.podopen);
						btnPod3.setText("SIPAHI");
						
					}
					btnPod1.setClickable(false);
					btnPod2.setClickable(false);
					btnPod3.setClickable(false);
					btnPod4.setClickable(false);
					updateScore();
				}
			});
		}
    	
		
		Log.v("AkhandBakar","#########" + btnPod4.getText());
		if(btnPod4.getText().equals("")){
			
			btnPod4.setOnClickListener(new onClickListener() {
				
			
				public void onClick(View v) {
					// TODO Auto-generated method stub
					Log.v("AkhandBakar","#########" + player_four);
					if(player_four.equals("CHOR")){
					
						RajaMantri.guess = true;
						btnPod4.setBackgroundResource(R.drawable.podopen);
						btnPod4.setText("CHOR");
					}else{
						
						RajaMantri.guess = false;
						btnPod4.setBackgroundResource(R.drawable.podopen);
						btnPod4.setText("SIPAHI");
						
					}
					btnPod1.setClickable(false);
					btnPod2.setClickable(false);
					btnPod3.setClickable(false);
					btnPod4.setClickable(false);
					updateScore();
				}
			});
		}
		
    }
    
    
    public void shuffle(){
    	
    	btnPlay.setText("Guess");
			btnPlay.setClickable(false);
			shuffleArray(solutionArray);
			txtTurn.setText(player_one_name + "'s" + " turn!");
			nextTurn = player_two_name;
			btnPod1 = (Button)findViewById(R.id.btnPod1);
			btnPod1.setBackgroundResource(R.drawable.podtlclosed);
			btnPod1.setOnClickListener(new onClickListener() {
				
				public void onClick(View v) {
					// TODO Auto-generated method stub
					player_one = solutionArray[0];
					btnPod1.setText(player_one);
					btnPod1.setBackgroundResource(R.drawable.podopen);
					btnPod2.setClickable(false);
					btnPod3.setClickable(false);
					btnPod4.setClickable(false);
					if(txtTurn.getText().equals(player_one_name + "'s" + " turn!")){
						
						if(player_one.equals("MANTRI")){
							
							player_one_role = "MANTRI";
						}
						if(player_one.equals("RAJA")){
							
							player_one_role = "RAJA";
						}
						if(player_one.equals("SIPAHI")){

							player_one_role = "SIPAHI";
						}
						if(player_one.equals("CHOR")){
							
							player_one_role = "CHOR";
						}
				    	

						nextTurn = player_two_name + "'s" + " turn!";
						
					}
					if(txtTurn.getText().equals(player_two_name + "'s" + " turn!")){
						
						if(player_one.equals("MANTRI")){
							
							player_two_role = "MANTRI";
						}
						if(player_one.equals("RAJA")){
							
							player_two_role = "RAJA";
						}
						if(player_one.equals("SIPAHI")){

							player_two_role = "SIPAHI";
						}
						if(player_one.equals("CHOR")){
							
							player_two_role = "CHOR";
						}
				    	
						nextTurn = player_three_name + "'s" + " turn!";
						
					}
					if(txtTurn.getText().equals(player_three_name + "'s" + " turn!")){
						
						if(player_one.equals("MANTRI")){
							
							player_three_role = "MANTRI";
						}
						if(player_one.equals("RAJA")){
							
							player_three_role = "RAJA";
						}
						if(player_one.equals("SIPAHI")){

							player_three_role = "SIPAHI";
						}
						if(player_one.equals("CHOR")){
							
							player_three_role = "CHOR";
						}
				    	
						nextTurn = player_four_name + "'s" + " turn!";
						
					}
					
					if(txtTurn.getText().equals(player_four_name + "'s" + " turn!")){
						
						if(player_one.equals("MANTRI")){
							
							player_four_role = "MANTRI";
						}
						if(player_one.equals("RAJA")){
							
							player_four_role = "RAJA";
						}
						if(player_one.equals("SIPAHI")){

							player_four_role = "SIPAHI";
						}
						if(player_one.equals("CHOR")){
							
							player_four_role = "CHOR";
						}
				    	
						
						nextTurn = "Click on Guess!";
						
					}
					
					txtTurn.setText("Click again to close the chit!");
				
					
					
					btnPod1.setOnClickListener(new onClickListener() {
						
						public void onClick(View v) {
							
							btnPod1.setClickable(false);
							count++;
							btnPod1.setText("");
							btnPod1.setBackgroundResource(R.drawable.podtlhalf);
							txtTurn.setText(nextTurn);
							btnPod2.setClickable(true);
							btnPod3.setClickable(true);
							btnPod4.setClickable(true);
							if(count == 4){
								
								txtTurn.setText("Click on Guess!");
								btnPlay.setClickable(true);
								count = 0;
								
							}
						}
					});
				}
			});
			
			btnPod2 = (Button)findViewById(R.id.btnPod2);
			btnPod2.setBackgroundResource(R.drawable.podtrclosed);
			btnPod2.setOnClickListener(new onClickListener() {
					
					public void onClick(View v) {
						
						player_two = solutionArray[1];
						btnPod2.setText(player_two);
						btnPod2.setBackgroundResource(R.drawable.podopen);
						btnPod1.setClickable(false);
						btnPod3.setClickable(false);
						btnPod4.setClickable(false);
						if(txtTurn.getText().equals(player_one_name + "'s" + " turn!")){
							
							if(player_two.equals("MANTRI")){
								
								player_one_role = "MANTRI";
							}
							if(player_two.equals("RAJA")){
								
								player_one_role = "RAJA";
							}
							if(player_two.equals("SIPAHI")){

								player_one_role = "SIPAHI";
							}
							if(player_two.equals("CHOR")){
								
								player_one_role = "CHOR";
							}
					    	
							nextTurn = player_two_name+ "'s" + " turn!";
							
						}
						if(txtTurn.getText().equals(player_two_name + "'s" + " turn!")){
							
							if(player_two.equals("MANTRI")){
								
								player_two_role = "MANTRI";
							}
							if(player_two.equals("RAJA")){
								
								player_two_role = "RAJA";
							}
							if(player_two.equals("SIPAHI")){

								player_two_role = "SIPAHI";
							}
							if(player_two.equals("CHOR")){
								
								player_two_role = "CHOR";
							}
					    	
							nextTurn = player_three_name+ "'s" + " turn!";
							
						}
						if(txtTurn.getText().equals(player_three_name + "'s" + " turn!")){
							
							if(player_two.equals("MANTRI")){
								
								player_three_role = "MANTRI";
							}
							if(player_two.equals("RAJA")){
								
								player_three_role = "RAJA";
							}
							if(player_two.equals("SIPAHI")){

								player_three_role = "SIPAHI";
							}
							if(player_two.equals("CHOR")){
								
								player_three_role = "CHOR";
							}
					    	
							nextTurn = player_four_name+ "'s" + " turn!";
							
						}
						if(txtTurn.getText().equals(player_four_name + "'s" + " turn!")){
							
							if(player_two.equals("MANTRI")){
								
								player_four_role = "MANTRI";
							}
							if(player_two.equals("RAJA")){
								
								player_four_role = "RAJA";
							}
							if(player_two.equals("SIPAHI")){

								player_four_role = "SIPAHI";
							}
							if(player_two.equals("CHOR")){
								
								player_four_role = "CHOR";
							}
					    	
							nextTurn = "Click on Guess!";
							
						}
						txtTurn.setText("Click again to close the chit!");
						btnPod2.setOnClickListener(new onClickListener() {
							
							public void onClick(View v) {
								// TODO Auto-generated method stub
								btnPod2.setClickable(false);
								count++;
								btnPod2.setText("");
								btnPod2.setBackgroundResource(R.drawable.podtrhalf);
								txtTurn.setText(nextTurn);
								btnPod1.setClickable(true);
								btnPod3.setClickable(true);
								btnPod4.setClickable(true);
								if(count == 4){
									
									txtTurn.setText("Click on Guess!");
									btnPlay.setClickable(true);
									count = 0;
									
								}
							}
						});
					}
				});
		        
		        
			btnPod3 = (Button)findViewById(R.id.btnPod3);
			btnPod3.setBackgroundResource(R.drawable.podblclosed);
			btnPod3.setOnClickListener(new onClickListener() {
					
					public void onClick(View v) {
						// TODO Auto-generated method stub
						player_three = solutionArray[2];
						btnPod3.setText(player_three);
						btnPod3.setBackgroundResource(R.drawable.podopen);

						btnPod2.setClickable(false);
						btnPod1.setClickable(false);
						btnPod4.setClickable(false);
						if(txtTurn.getText().equals(player_one_name + "'s" + " turn!")){
							
							if(player_three.equals("MANTRI")){
								
								player_one_role = "MANTRI";
							}
							if(player_three.equals("RAJA")){
								
								player_one_role = "RAJA";
							}
							if(player_three.equals("SIPAHI")){

								player_one_role = "SIPAHI";
							}
							if(player_three.equals("CHOR")){
								
								player_one_role = "CHOR";
							}
					    	
							nextTurn = player_two_name+ "'s" + " turn!";
							
						}
						if(txtTurn.getText().equals(player_two_name + "'s" + " turn!")){
							
							if(player_three.equals("MANTRI")){
								
								player_two_role = "MANTRI";
							}
							if(player_three.equals("RAJA")){
								
								player_two_role = "RAJA";
							}
							if(player_three.equals("SIPAHI")){

								player_two_role = "SIPAHI";
							}
							if(player_three.equals("CHOR")){
								
								player_two_role = "CHOR";
							}
					    	
							nextTurn = player_three_name+ "'s" + " turn!";
							
						}
						if(txtTurn.getText().equals(player_three_name + "'s" + " turn!")){
							
							if(player_three.equals("MANTRI")){
								
								player_three_role = "MANTRI";
							}
							if(player_three.equals("RAJA")){
								
								player_three_role = "RAJA";
							}
							if(player_three.equals("SIPAHI")){

								player_three_role = "SIPAHI";
							}
							if(player_three.equals("CHOR")){
								
								player_three_role = "CHOR";
							}
							nextTurn = player_four_name+ "'s" + " turn!";
							
						}
						if(txtTurn.getText().equals(player_four_name + "'s" + " turn!")){
							
							if(player_three.equals("MANTRI")){
								
								player_four_role = "MANTRI";
							}
							if(player_three.equals("RAJA")){
								
								player_four_role = "RAJA";
							}
							if(player_three.equals("SIPAHI")){

								player_four_role = "SIPAHI";
							}
							if(player_three.equals("CHOR")){
								
								player_four_role = "CHOR";
							}
							nextTurn = "Click on Guess!";
							
						}

						txtTurn.setText("Click again to close the chit!");
						btnPod3.setOnClickListener(new onClickListener() {
							
							public void onClick(View v) {
								// TODO Auto-generated method stub
								btnPod3.setClickable(false);
								count++;
								btnPod3.setText("");
								btnPod3.setBackgroundResource(R.drawable.podblhalf);
								txtTurn.setText(nextTurn);
								btnPod2.setClickable(true);
								btnPod1.setClickable(true);
								btnPod4.setClickable(true);
								if(count == 4){
									
									txtTurn.setText("Click on Guess!");
									btnPlay.setClickable(true);
									count = 0;
									
								}
							}
						});
					}
				});
		     
			
			
			
			btnPod4 = (Button)findViewById(R.id.btnPod4);
			btnPod4.setBackgroundResource(R.drawable.podbrclosed);
			
			btnPod4.setOnClickListener(new onClickListener() {
					
					public void onClick(View v) {
						// TODO Auto-generated method stub
						player_four = solutionArray[3];
						btnPod4.setText(player_four);
						btnPod4.setBackgroundResource(R.drawable.podopen);
						

						btnPod2.setClickable(false);
						btnPod3.setClickable(false);
						btnPod1.setClickable(false);
						if(txtTurn.getText().equals(player_one_name + "'s" + " turn!")){
							
							if(player_four.equals("MANTRI")){
								
								player_one_role = "MANTRI";
							}
							if(player_four.equals("RAJA")){
								
								player_one_role = "RAJA";
							}
							if(player_four.equals("SIPAHI")){

								player_one_role = "SIPAHI";
							}
							if(player_four.equals("CHOR")){
								
								player_one_role = "CHOR";
							}
							nextTurn = player_two_name+ "'s" + " turn!";
							
						}
						if(txtTurn.getText().equals(player_two_name + "'s" + " turn!")){
							
							if(player_four.equals("MANTRI")){
								
								player_two_role = "MANTRI";
							}
							if(player_four.equals("RAJA")){
								
								player_two_role = "RAJA";
							}
							if(player_four.equals("SIPAHI")){

								player_two_role = "SIPAHI";
							}
							if(player_four.equals("CHOR")){
								
								player_two_role = "CHOR";
							}
							nextTurn = player_three_name+ "'s" + " turn!";
							
						}
						if(txtTurn.getText().equals(player_three_name + "'s" + " turn!")){
							
							if(player_four.equals("MANTRI")){
								
								player_three_role = "MANTRI";
							}
							if(player_four.equals("RAJA")){
								
								player_three_role = "RAJA";
							}
							if(player_four.equals("SIPAHI")){

								player_three_role = "SIPAHI";
							}
							if(player_four.equals("CHOR")){
								
								player_three_role = "CHOR";
							}
							nextTurn = player_four_name+ "'s" + " turn!";
							
						}
						if(txtTurn.getText().equals(player_four_name + "'s" + " turn!")){
							
							if(player_four.equals("MANTRI")){
								
								player_four_role = "MANTRI";
							}
							if(player_four.equals("RAJA")){
								
								player_four_role = "RAJA";
							}
							if(player_four.equals("SIPAHI")){

								player_four_role = "SIPAHI";
							}
							if(player_four.equals("CHOR")){
								
								player_four_role = "CHOR";
							}
							nextTurn = "Click on Guess!";
							
						}
						
						txtTurn.setText("Click again to close the chit!");
						btnPod4.setOnClickListener(new onClickListener() {
							
							public void onClick(View v) {
								// TODO Auto-generated method stub
								btnPod4.setClickable(false);
								count++;
								btnPod4.setText("");
								btnPod4.setBackgroundResource(R.drawable.podbrhalf);
								txtTurn.setText(nextTurn);
								btnPod2.setClickable(true);
								btnPod3.setClickable(true);
								btnPod1.setClickable(true);
								if(count == 4){
									
									txtTurn.setText(nextTurn);
									btnPlay.setClickable(true);
									count = 0;
									
								}
							}
						});
					}
				});    
			
			btnPod1.setText("");
			btnPod2.setText("");
			btnPod3.setText("");
			btnPod4.setText("");
    	
    	
    }
    
    public void setRole(String role, String player){
    	
    	if(player_one.equals("MANTRI")){
			
			player_four_role = "MANTRI";
		}
		if(player_one.equals("RAJA")){
			
			player_four_role = "RAJA";
		}
		if(player_one.equals("SIPAHI")){

			player_four_role = "SIPAHI";
		}
		if(player_one.equals("CHOR")){
			
			player_four_role = "CHOR";
		}
    	
    	
    } 
    
    void shuffleArray(String[] solutionArray)
    {
    	Random rnd = new Random();
    	for (int i = solutionArray.length - 1; i >= 0; i--)
    		{
    			int index = rnd.nextInt(i + 1);
  
    			String a = solutionArray[index];
    			solutionArray[index] = solutionArray[i];
    			solutionArray[i] = a;
    		}
	}
    
    static void updateScore(){
    	
    	Log.v("AkhandBakar", "##########"+ guess);
    	if(player_one_role.equals("MANTRI"))
    	{
    		Log.v("AkhandBakar", "##########Mantri"+ player_one_name);
    	if(guess)
    		{
    		i = i+80;
    		p_one_score=i;
    		txtTurn.setText(player_one_name+" is right!");
    		btnPod1.setText(player_one);
			btnPod2.setText(player_two);
			btnPod3.setText(player_three);
			btnPod4.setText(player_four);
			btnPod1.setBackgroundResource(R.drawable.podopen);
			btnPod2.setBackgroundResource(R.drawable.podopen);
			btnPod3.setBackgroundResource(R.drawable.podopen);
			btnPod4.setBackgroundResource(R.drawable.podopen);
    		if(player_two_role.equals("CHOR"))
    			{
    			p_two_score=j;
    			if(player_three_role.equals("RAJA")){
    				
    				k = k+100;
    				l = l+50;
    				p_three_score=k;
    				p_four_score=l;
    			}else{
    				
    				l = l+100;
    				k = k+50;
    				p_four_score=l;
    				p_three_score=k;
    			}
    			}
    		if(player_three_role.equals("CHOR"))
    			{
    			
    			p_three_score=k;
    			
    			
    			if(player_two_role.equals("RAJA")){
    				
    				j = j+100;
    				l = l+50;
    				p_two_score=j;
    				p_four_score=l;
    			}else{
    				
    				l = l+100;
    				j = j+50;
    				p_four_score=l;
    				p_two_score=j;
    			}
    			}
    		if(player_four_role.equals("CHOR"))
    			{
    			
    			p_four_score=l;
    			
    			if(player_three_role.equals("RAJA")){
    				
    				k = k+100;
    				j = j+50;
    				p_two_score=j;
    				p_three_score=k;
    			}else{
    				
    				j = j+100;
    				k = k+50;
    				p_three_score=k;
    				p_two_score=j;
    			}
    			}
    		}
    	else
    		{
    		i=i-80;
    		p_one_score = i;
    		txtTurn.setText(player_one_name+" is wrong!");
    		btnPod1.setText(player_one);
			btnPod2.setText(player_two);
			btnPod3.setText(player_three);
			btnPod4.setText(player_four);
			btnPod1.setBackgroundResource(R.drawable.podopen);
			btnPod2.setBackgroundResource(R.drawable.podopen);
			btnPod3.setBackgroundResource(R.drawable.podopen);
			btnPod4.setBackgroundResource(R.drawable.podopen);
			if(player_two_role.equals("CHOR"))
			{
				j = j+25;
			p_two_score=j;
			if(player_three_role.equals("RAJA")){
				
				k = k+100;
				l = l+50;
				p_three_score=k;
				p_four_score=l;
			}else{
				
				l = l+100;
				k = k+50;
				p_four_score=l;
				p_three_score=k;
			}
			}
		if(player_three_role.equals("CHOR"))
			{
			k=k+25;
			p_three_score=k;
			
			
			if(player_two_role.equals("RAJA")){
				
				j = j+100;
				l = l+50;
				p_two_score=j;
				p_four_score=l;
			}else{
				
				l = l+100;
				j = j+50;
				p_four_score=l;
				p_two_score=j;
			}
			}
		if(player_four_role.equals("CHOR"))
			{
			l=l+25;
			p_four_score=l;
			
			if(player_three_role.equals("RAJA")){
				
				k = k+100;
				j = j+50;
				p_two_score=j;
				p_three_score=k;
			}else{
				
				j = j+100;
				k = k+50;
				p_three_score=k;
				p_two_score=j;
			}
			}
    		}

    	}
    if(player_two_role.equals("MANTRI"))
    	{
    	if(guess)
    		{
    		Log.v("AkhandBakar", "##########Mantri"+ player_two_name);
    		j = j+80;
    		p_two_score=j;
    		txtTurn.setText(player_two_name+" is right!");
    		btnPod1.setText(player_one);
			btnPod2.setText(player_two);
			btnPod3.setText(player_three);
			btnPod4.setText(player_four);
			btnPod1.setBackgroundResource(R.drawable.podopen);
			btnPod2.setBackgroundResource(R.drawable.podopen);
			btnPod3.setBackgroundResource(R.drawable.podopen);
			btnPod4.setBackgroundResource(R.drawable.podopen);
    		if(player_one_role.equals("CHOR"))
    			{
    			p_one_score=i;
    			
    			if(player_three_role.equals("RAJA")){
    			
    				k = k+100;
    				l = l+50;
    				p_three_score=k;
    				p_four_score=l;
    			
    			}else{
    				
    				l = l+100;
    				k = k+50;
    				p_four_score=l;
    				p_three_score=k;
    			}
    			
    			}
    		if(player_three_role.equals("CHOR"))
    			{
    			
    			p_three_score=k;
    			
    			
    			if(player_one_role.equals("RAJA")){
    				
    				i = i+100;
    				l = l+50;
    				p_one_score=i;
    				p_four_score=l;
    				
    			}else{
    				
    				l = l+100;
    				i = i+50;
    				p_one_score=i;
    				p_four_score=l;
    				
    			}
    			
    			}
    		if(player_four_role.equals("CHOR"))
    			{
    			
    			p_four_score=l;
    			
    			if(player_one_role.equals("RAJA")){
    				
    				i = i+100;
    				k = k+50;
    				p_one_score=i;
        			p_three_score=k;
    				
    			}else{
    				
    				k = k+100;
    				i = i+50;
    				p_one_score=i;
        			p_three_score=k;
    			
    			
    			}
    			
    			
    			}
    		}
    	else
    		{
    		 
    		j=j-80;
    		p_two_score = j;
    		txtTurn.setText(player_two_name+" is wrong!");
    		btnPod1.setText(player_one);
			btnPod2.setText(player_two);
			btnPod3.setText(player_three);
			btnPod4.setText(player_four);
			btnPod1.setBackgroundResource(R.drawable.podopen);
			btnPod2.setBackgroundResource(R.drawable.podopen);
			btnPod3.setBackgroundResource(R.drawable.podopen);
			btnPod4.setBackgroundResource(R.drawable.podopen);
			if(player_one_role.equals("CHOR"))
			{
				i = i+25;
			p_one_score=i;
			
			if(player_three_role.equals("RAJA")){
			
				k = k+100;
				l = l+50;
				p_three_score=k;
				p_four_score=l;
			
			}else{
				
				l = l+100;
				k = k+50;
				p_four_score=l;
				p_three_score=k;
			}
			
			}
		if(player_three_role.equals("CHOR"))
			{
			k = k+25;
			p_three_score=k;
			
			
			if(player_one_role.equals("RAJA")){
				
				i = i+100;
				l = l+50;
				p_one_score=i;
				p_four_score=l;
				
			}else{
				
				l = l+100;
				i = i+50;
				p_one_score=i;
				p_four_score=l;
				
			}
			
			}
		if(player_four_role.equals("CHOR"))
			{
			l = l+25;
			p_four_score=l;
			
			if(player_one_role.equals("RAJA")){
				
				i = i+100;
				k = k+50;
				p_one_score=i;
    			p_three_score=k;
				
			}else{
				
				k = k+100;
				i = i+50;
				p_one_score=i;
    			p_three_score=k;
			
			
			}
			
			
			}
    		}

    	}
    if(player_three_role.equals("MANTRI"))
    	{
    	Log.v("AkhandBakar", "##########Mantri"+ player_three_name);
    	if(guess)
    		{
    		k = k+80;
    		p_three_score = k;
    		txtTurn.setText(player_three_name+" is right!");
    		btnPod1.setText(player_one);
			btnPod2.setText(player_two);
			btnPod3.setText(player_three);
			btnPod4.setText(player_four);
			btnPod1.setBackgroundResource(R.drawable.podopen);
			btnPod2.setBackgroundResource(R.drawable.podopen);
			btnPod3.setBackgroundResource(R.drawable.podopen);
			btnPod4.setBackgroundResource(R.drawable.podopen);
    		if(player_one_role.equals("CHOR"))
    			{
    			p_one_score=i;
    			
    			if(player_two_role.equals("RAJA")){
    				
    				j = j+100;
    				l = l+50;
    				p_two_score=j;
        			p_four_score=l;
        			
    				
    			}else{
    				
    				l = l+100;
    				j = j+50;
    				p_two_score=j;
        			p_four_score=l;
    				
    				
    			}
    			
    			}
    		if(player_two_role.equals("CHOR"))
    			{
    			
    			p_two_score=j;
    			
    			
    			if(player_one_role.equals("RAJA")){
    				
    				i = i+100;
    				l = l+50;
    				p_one_score=i;
    				p_four_score=l;
    				
    			}else{
    				
    				i = i+50;
    				l = l+100;
    				p_one_score=i;
    				p_four_score=l;
    				
    			}
    			
    			}
    		if(player_four_role.equals("CHOR"))
    			{
    			
    			p_four_score=l;
    			
    			if(player_two_role.equals("RAJA")){
    				
    				j = j+100;
    				i = i+50;
    				p_one_score=i;
        			p_two_score=j;
    				
    			}else{
    				
    				j = j+50;
    				i = i+100;
    				p_one_score=i;
        			p_two_score=j;
    				
    			}
    			
    			
    			}
    		}
    	else
    		{
    		k = k-80;
    		p_three_score = k;
    		txtTurn.setText(player_three_name+" is wrong!");
    		btnPod1.setText(player_one);
			btnPod2.setText(player_two);
			btnPod3.setText(player_three);
			btnPod4.setText(player_four);
			btnPod1.setBackgroundResource(R.drawable.podopen);
			btnPod2.setBackgroundResource(R.drawable.podopen);
			btnPod3.setBackgroundResource(R.drawable.podopen);
			btnPod4.setBackgroundResource(R.drawable.podopen);
			if(player_one_role.equals("CHOR"))
			{
				i = i+25;
			p_one_score=i;
			
			if(player_two_role.equals("RAJA")){
				
				j = j+100;
				l = l+50;
				p_two_score=j;
    			p_four_score=l;
    			
				
			}else{
				
				l = l+100;
				j = j+50;
				p_two_score=j;
    			p_four_score=l;
				
				
			}
			
			}
		if(player_two_role.equals("CHOR"))
			{
			j = j+25;
			p_two_score=j;
			
			
			if(player_one_role.equals("RAJA")){
				
				i = i+100;
				l = l+50;
				p_one_score=i;
				p_four_score=l;
				
			}else{
				
				i = i+50;
				l = l+100;
				p_one_score=i;
				p_four_score=l;
				
			}
			
			}
		if(player_four_role.equals("CHOR"))
			{
			l = l+25;
			p_four_score=l;
			
			if(player_two_role.equals("RAJA")){
				
				j = j+100;
				i = i+50;
				p_one_score=i;
    			p_two_score=j;
				
			}else{
				
				j = j+50;
				i = i+100;
				p_one_score=i;
    			p_two_score=j;
				
			}
			
			
			}
    		}

    	}
    if(player_four_role.equals("MANTRI"))
    	{
    	Log.v("AkhandBakar", "##########Mantri"+ player_four_name);
    	if(guess)
    		{
    		l = l+80;
    		p_four_score=l;
    		txtTurn.setText(player_four_name+" is right!");
    		btnPod1.setText(player_one);
			btnPod2.setText(player_two);
			btnPod3.setText(player_three);
			btnPod4.setText(player_four);
			btnPod1.setBackgroundResource(R.drawable.podopen);
			btnPod2.setBackgroundResource(R.drawable.podopen);
			btnPod3.setBackgroundResource(R.drawable.podopen);
			btnPod4.setBackgroundResource(R.drawable.podopen);
    		if(player_one_role.equals("CHOR"))
    			{
    			p_one_score=i;
    			
    			
    			if(player_two_role.equals("RAJA")){
    				
    				j = j+100;
    				k = k+50;
    				p_two_score=j;
        			p_three_score=k;
    				
    			}else{
    				
    				j = j+50;
    				k = k+100;
    				p_two_score=j;
        			p_three_score=k;
    				
    			}
    			}
    		if(player_two_role.equals("CHOR"))
    			{
    			
    			p_two_score=j;
    			
    			
    			if(player_one_role.equals("RAJA")){
    				
    				i = i+100;
    				k = k+50;
    				p_one_score=i;
    				p_three_score=k;
    			}else{
    				
    				i = i+50;
    				k = k+100;
    				p_one_score=i;
    				p_three_score=k;
    				
    			}
    			
    			}
    		if(player_three_role.equals("CHOR"))
    			{
    			
    			p_three_score=k;
    			
    			if(player_one_role.equals("RAJA")){
    				
    				i = i+100;
    				j = j+50;
    				p_one_score=i;
        			p_two_score=j;
    			}else{
    				
    				i = i+50;
    				j = j+100;
    				p_one_score=i;
        			p_two_score=j;
    				
    			}
    			
    			
    			}
    		}
    	else
    		{
    		l = l-80;
    		p_four_score = l;
    		txtTurn.setText(player_four_name+" is wrong!");
    		btnPod1.setText(player_one);
			btnPod2.setText(player_two);
			btnPod3.setText(player_three);
			btnPod4.setText(player_four);
			btnPod1.setBackgroundResource(R.drawable.podopen);
			btnPod2.setBackgroundResource(R.drawable.podopen);
			btnPod3.setBackgroundResource(R.drawable.podopen);
			btnPod4.setBackgroundResource(R.drawable.podopen);
			if(player_one_role.equals("CHOR"))
			{
				i = i+25;
			p_one_score=i;
			
			
			if(player_two_role.equals("RAJA")){
				
				j = j+100;
				k = k+50;
				p_two_score=j;
    			p_three_score=k;
				
			}else{
				
				j = j+50;
				k = k+100;
				p_two_score=j;
    			p_three_score=k;
				
			}
			}
		if(player_two_role.equals("CHOR"))
			{
			j=j+25;
			p_two_score=j;
			
			
			if(player_one_role.equals("RAJA")){
				
				i = i+100;
				k = k+50;
				p_one_score=i;
				p_three_score=k;
			}else{
				
				i = i+50;
				k = k+100;
				p_one_score=i;
				p_three_score=k;
				
			}
			
			}
		if(player_three_role.equals("CHOR"))
			{
			k=k+25;
			p_three_score=k;
			
			if(player_one_role.equals("RAJA")){
				
				i = i+100;
				j = j+50;
				p_one_score=i;
    			p_two_score=j;
			}else{
				
				i = i+50;
				j = j+100;
				p_one_score=i;
    			p_two_score=j;
				
			}
			
			
			}
    		}

    	}
    	
    
    Log.v("AkhandBakar", "##########Score "+ i);
	txtplayer_one.setText("1."+ player_one_name + " [" + i + "]");
	Log.v("AkhandBakar", player_one + " [" + i + "]");
	
	txtplayer_two.setText("2." + player_two_name+ " [" + j + "]");
	
	Log.v("AkhandBakar", player_two + " [" + p_two_score + "]");
	
	txtplayer_three.setText("3." + player_three_name+ " [" + k + "]");
	Log.v("AkhandBakar", player_three + " [" + p_three_score + "]");
	
	txtplayer_four.setText("4."+player_four_name+ " [" + l + "]");	
	Log.v("AkhandBakar", player_four + " [" + p_four_score + "]");
    }
}
