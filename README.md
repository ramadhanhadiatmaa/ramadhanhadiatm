A simple library to use Admob Native Ads in Android RecyclerView

Add admob native ads more easy to your recyclerview.

How to use :

Step 1 :

Add this at the top level gradle file :

    repositories {
    	maven { url "https://jitpack.io" }
    }

Step 2 : 

Add this in your app level gradle dependencies file :

    implementation 'com.github.kodlitecom:AdmobAdvancedNativeRecycler:1.0.2'

Step 3 :
Build the native Ad adapter from your current RecyclerView adapter :

    AdmobNativeAdAdapter admobNativeAdAdapter=AdmobNativeAdAdapter.Builder
    	.with(
    		nativeAdId,//Create a native ad id from admob console
    		currentAdapter,//The adapter you would normally set to your recyClerView
    		NativeAdsType//Set it with "small","medium" or "custom"
    		)
    	.adItemIterval(interval)//native ad repeating interval in the recyclerview
    	.build();
    recyclerView.setAdapter(admobNativeAdAdapter);//set your RecyclerView adapter with the admobNativeAdAdapter
    
This library from https://github.com/daoibrahim/AdmobAdvancedNativeRecyclerview

Enjoy!!!
