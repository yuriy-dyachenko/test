Totango Java API

	* getting track instance from any point of code
		Totango.getInstance(String serviceId);
	
	* identifying user and company for further tracking without specifying user and company
		identify(String org, String user)
		
	* tracking 
		track(String org, String user, String activity, String module)
		
		track(String activity, String module)
			NOTE: 	Identify user before calling this method otherwise UserNotIdentified exception will raise
	
	* seetting account attributes
		setAttributes(Map<String, String> attributes)
			NOTE: 	Attributes are map entries ("key":"value")
					Identify user before calling this method otherwise UserNotIdentified exception will raise

	* setting foreign id
		setForeignId(String foreignId)
			NOTE: 	Identify user before calling this method otherwise UserNotIdentified exception will raise
			
	* setting display name
		setDisplayName(String displayName)
			NOTE: 	Display name length should be up to 128 chars otherwise ExceededLengthValue exception will raise
					Identify user before calling this method otherwise UserNotIdentified exception will raise