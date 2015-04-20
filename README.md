
package karto.nik.service.objekt;

import javax.xml.bind.annotation.XmlRootElement;

@XmlRootElement
//Basisklasse für Zwischenspeicherung der Daten
//Ausgehend von der xml datei von Benedikt
public class NetworkStats {

	//Networkstats
	private String ProviderName;
	private int ASUValue;
	private int RSSIValue;
	private int NetworkID;
	private String NetworkType;
	//GPS
	private float Langitude;
	private float Longitude;
	
	//Getter und Setter
	
	public float getLangitude() {
		return Langitude;
	}
	public void setLangitude(float langitude) {
		Langitude = langitude;
	}
	public float getLongitude() {
		return Longitude;
	}
	public void setLongitude(float longitude) {
		Longitude = longitude;
	}
	public String getProviderName() {
		return ProviderName;
	}
	public void setProviderName(String providerName) {
		ProviderName = providerName;
	}
	public int getASUValue() {
		return ASUValue;
	}
	public void setASUValue(int aSUValue) {
		ASUValue = aSUValue;
	}
	public int getRSSIValue() {
		return RSSIValue;
	}
	public void setRSSIValue(int rSSIValue) {
		RSSIValue = rSSIValue;
	}
	public int getNetworkID() {
		return NetworkID;
	}
	public void setNetworkID(int networkID) {
		NetworkID = networkID;
	}
	public String getNetworkType() {
		return NetworkType;
	}
	public void setNetworkType(String networkType) {
		NetworkType = networkType;
	}
	
	//Konstruktoren
	
	public NetworkStats(){}
	
	public NetworkStats(String provider,int asuvvalue, int rssivalue,int networkid, String networktype, float langitude,float longitude){
		this.ProviderName=provider;
		this.ASUValue=asuvvalue;
		this.RSSIValue=rssivalue;
		this.NetworkID=networkid;
		this.NetworkType=networktype;
		this.Langitude=langitude;
		this.Longitude=longitude;
	}
}

