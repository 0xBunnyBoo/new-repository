import { ecosystemWallet } from "thirdweb/wallets";

const restrictedWallet = ecosystemWallet("ecosystem.xai-connect", {
	partnerId: "..." // partner ID provided to you by XAI
});
<ConnectButton
	client={THIRDWEB_CLIENT} /* your own thirdweb API key */
	wallets={[wallet]}
	{...props}
/>
<ConnectButton
	client={THIRDWEB_CLIENT} /* your own thirdweb API key */
	wallets={[inAppWallet(), createWallet("io.metamask"), createWallet("ecosystem.xai.connect")]}
	{...props}
/>
