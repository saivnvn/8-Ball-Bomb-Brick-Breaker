import SwiftUI

struct AboutView: View {
    
    let youtubeURL = URL(string: "https://studio.youtube.com/video/4NlTBXMbjAg/edit")!
    let appStoreURL = URL(string: "https://apps.apple.com/us/app/brick-breaker-8-ball-bomb/id6760389867")!
    
    var body: some View {
        ScrollView {
            
            VStack(spacing: 24) {
                
                // Logo
                Image("logo")
                    .resizable()
                    .scaledToFit()
                    .frame(width: 140)
                    .padding(.top, 20)
                
                // Title
                Text("8 Ball Bomb – Brick Breaker")
                    .font(.largeTitle)
                    .fontWeight(.bold)
                    .multilineTextAlignment(.center)
                
                Text("Shoot Balls. Break Bricks. Survive the Chaos.")
                    .font(.headline)
                    .foregroundColor(.secondary)
                    .multilineTextAlignment(.center)
                
                Divider()
                
                // Description
                Text("""
                8 Ball Bomb – Brick Breaker delivers an explosive twist on the classic brick breaker arcade game.

                Aim carefully and launch powerful balls to destroy descending numbered bricks before they reach the bottom.

                With smooth physics, satisfying explosions, and unpredictable power-ups, every round becomes a fast-paced arcade challenge.
                """)
                .font(.body)
                .multilineTextAlignment(.leading)
                
                Divider()
                
                // Screenshots
                VStack(alignment: .leading, spacing: 12) {
                    
                    Text("Screenshots")
                        .font(.title2)
                        .fontWeight(.bold)
                    
                    ScrollView(.horizontal, showsIndicators: false) {
                        HStack(spacing: 16) {
                            
                            Image("anh1")
                                .resizable()
                                .scaledToFit()
                                .frame(width: 220)
                                .cornerRadius(12)
                            
                            Image("anh2")
                                .resizable()
                                .scaledToFit()
                                .frame(width: 220)
                                .cornerRadius(12)
                            
                            Image("anh3")
                                .resizable()
                                .scaledToFit()
                                .frame(width: 220)
                                .cornerRadius(12)
                        }
                    }
                }
                
                Divider()
                
                // Features
                VStack(alignment: .leading, spacing: 12) {
                    
                    Text("Features")
                        .font(.title2)
                        .fontWeight(.bold)
                    
                    FeatureRow(text: "Aim and shoot 8 powerful balls")
                    FeatureRow(text: "Destroy descending numbered bricks")
                    FeatureRow(text: "Random power-ups like Double Damage")
                    FeatureRow(text: "Massive 16 Ball Storm bonus")
                    FeatureRow(text: "Smooth physics and satisfying explosions")
                    FeatureRow(text: "Endless difficulty challenge")
                    FeatureRow(text: "Global leaderboard competition")
                }
                
                Divider()
                
                // Buttons
                VStack(spacing: 12) {
                    
                    Link("Watch Gameplay Video", destination: youtubeURL)
                        .buttonStyle(.borderedProminent)
                    
                    Link("Download on the App Store", destination: appStoreURL)
                        .buttonStyle(.bordered)
                }
                
                Spacer(minLength: 30)
            }
            .padding()
        }
    }
}

struct FeatureRow: View {
    
    let text: String
    
    var body: some View {
        HStack(alignment: .top) {
            Image(systemName: "circle.fill")
                .font(.system(size: 8))
                .padding(.top, 6)
            
            Text(text)
        }
    }
}

#Preview {
    AboutView()
}
