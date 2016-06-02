#_Flying_Object
public_class_Flyer_{
	private_double_airSpeedMilesPerMinute;
	private_int_elevationPerMinute;
	private_int_totalAltitude_=_0;
	private_double_totalDistance_=_0;
	
	public_Flyer(){
		this.airSpeedMilesPerMinute_=_0;
		this.elevationPerMinute_=_0;
	}
	public_Flyer(int_airSpeedMPH,_int_elevationPerMinute){
		this.airSpeedMilesPerMinute_=_(double)airSpeedMPH_/_60;
		this.elevationPerMinute_=_elevationPerMinute;
	}
	public_void_SetAirSpeed(int airSpeedMPH){
		this.airSpeedMilesPerMinute_=_(double)airSpeedMPH_/_60;
	}
	public_void_SetAltimeter(int_elevationPerMinute){
		this.elevationPerMinute_=_elevationPerMinute;
	}
	public_void_Fly(){
		this.totalAltitude_= _his.totalAltitude_+_this.elevationPerMinute;
		this.totalDistance_=_this.totalDistance_+_this.airSpeedMilesPerMinute;
	}
	public_String_toString(){
		return_"Distance Flown:"_+_this.totalDistance_+";_Current Altitude:_"+_this.totalAltitude;
	}
}
