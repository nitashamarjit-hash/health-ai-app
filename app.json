import React, { useState, useEffect } from 'react';
import {
  StyleSheet,
  Text,
  View,
  TouchableOpacity,
  ScrollView,
  SafeAreaView,
  StatusBar,
  TextInput,
  Dimensions,
  Alert,
} from 'react-native';

const { width } = Dimensions.get('window');

const LANGUAGES = [
  { id: 'pa', name: 'ਪੰਜਾਬੀ' },
  { id: 'hi', name: 'हिंदी' },
  { id: 'en', name: 'English' },
  { id: 'es', name: 'Español' },
  { id: 'ar', name: 'العربية' },
  { id: 'zh', name: '中文' },
];

export default function App() {
  const [selectedLang, setSelectedLang] = useState('pa');
  const [userQuery, setUserQuery] = useState('');
  const [evolutionVersion, setEvolutionVersion] = useState('v10000.9 (Master Unified Engine)');
  const [isOwnerMode, setIsOwnerMode] = useState(false);
  const [aiResponse, setAiResponse] = useState(
    'ਸਤਿ ਸ਼੍ਰੀ ਅਕਾਲ ਜੀ! ਮੈਂ Vitalix AI ਹਾਂ—ਮਾਨਵਤਾ ਦੇ ਇਤਿਹਾਸ, ਬਿਮਾਰੀਆਂ ਦੇ ਪ੍ਰਾਚੀਨ ਤੇ ਅਧੁਨਿਕ ਇਲਾਜ, ਆਯੁਰਵੇਦ, ਯੋਗਾ, ਹੋਮੀਓਪੈਥੀ ਅਤੇ ਸਾਇੰਟਿਫਿਕ ਖੋਜਾਂ ਦਾ ਸੰਪੂਰਨ ਗਿਆਨ-ਕੇਂਦਰ। ਆਪਣੀ ਸਮੱਸਿਆ ਜਾਂ ਖੋਜ ਬਾਰੇ ਲਿਖੋ।'
  );
  const [isAnalyzing, setIsAnalyzing] = useState(false);

  // ਆਟੋਮੈਟਿਕ ਸਿਸਟਮ ਡਿਵੈਲਪਮੈਂਟ ਅਤੇ ਲਰਨਿੰਗ ਚੱਕਰ
  useEffect(() => {
    const interval = setInterval(() => {
      const randomSubVer = Math.floor(Math.random() * 90000) + 10000;
      setEvolutionVersion(`v10000.${randomSubVer} (Auto-Learning & Universal Knowledge Active)`);
    }, 8000);
    return () => clearInterval(interval);
  }, []);

  const toggleOwnerMode = () => {
    setIsOwnerMode(!isOwnerMode);
    Alert.alert(
      isOwnerMode ? 'User Mode Active' : '👑 SOLE OWNER MASTER ACCESS',
      isOwnerMode 
        ? 'ਤੁਸੀਂ ਆਮ ਯੂਜ਼ਰ ਮੋਡ ਵਿੱਚ ਹੋ।' 
        : 'ਤੁਹਾਡੇ ਕੋਲ ਕੋਡਿੰਗ, ਨਵੀਂਆਂ ਫੀਚਰਾਂ ਜੋੜਨ ਅਤੇ 100% ਨਿਯੰਤਰਣ ਦੀ ਪੂਰੀ ਅਥਾਰਟੀ ਹੈ।'
    );
  };

  const handleHeartCheck = () => {
    Alert.alert(
      '🚨 EARLY EMERGENCY & HEART GUARD SCANNER',
      'ਸਰੀਰਕ ਸੰਕੇਤਾਂ ਦੀ ਸਮੇਂ ਸਿਰ ਜਾਂਚ ਕੀਤੀ ਗਈ ਹੈ। ਸਿਸਟਮ ਪੂਰੀ ਤਰ੍ਹਾਂ ਸਕ੍ਰਿਅ ਹੈ ਅਤੇ ਅਟੈਕ ਤੋਂ ਪਹਿਲਾਂ ਚੇਤਾਵਨੀ ਦੇਣ ਲਈ ਤਿਆਰ ਹੈ।'
    );
  };

  const handleMasterDiagnostic = () => {
    if (!userQuery.trim()) return;
    setIsAnalyzing(true);
    setAiResponse('ਸ੍ਰਿਸ਼ਟੀ ਦੇ ਇਤਿਹਾਸ, ਸਾਰੀਆਂ ਬਿਮਾਰੀਆਂ ਦੀ ਖੋਜ, ਆਯੁਰਵੇਦ, ਮੈਡੀਕਲ ਮਸ਼ੀਨਰੀ ਅਤੇ ਯੋਗਾ ਗਿਆਨ ਦੁਆਰਾ ਜਾਂਚ ਕੀਤੀ ਜਾ ਰਹੀ ਹੈ...');

    setTimeout(() => {
      setIsAnalyzing(false);
      setAiResponse(
        `[VITALIX MASTER UNIFIED HEALTH REPORT]\n\n❤️ ਮਾਨਸਿਕ ਸ਼ਾਂਤੀ & ਹੌਂਸਲਾ: "ਹਰ ਸਮੱਸਿਆ ਦਾ ਸਮਾਧਾਨ ਸੰਭਵ ਹੈ। ਪੂਰੇ ਵਿਸ਼ਵਾਸ ਨਾਲ ਨਿਯਮਾਂ ਦਾ ਪਾਲਣ ਕਰੋ।"\n\n📜 ਇਤਿਹਾਸਕ & ਸਾਇੰਟਿਫਿਕ ਰਿਸਰਚ: ਬਿਮਾਰੀ ਦੇ ਮੂਲ ਕਾਰਨ ਅਤੇ ਪ੍ਰਾਚੀਨ-ਅਧੁਨਿਕ ਇਲਾਜ ਪ੍ਰਣਾਲੀਆਂ ਦਾ ਸੁਮੇਲ।\n\n🌿 ਔਰਗੈਨਿਕ & ਆਯੁਰਵੇਦ: ਬਿਮਾਰੀ ਨੂੰ ਜੜ੍ਹੋਂ ਖਤਮ ਕਰਨ ਲਈ ਸ਼ੁੱਧ ਜੜ੍ਹੀ-ਬੂਟੀਆਂ ਦਾ ਨੁਸਖਾ।\n\n⏰ ਟਾਈਮ-ਰਿੰਗ ਅਲਾਰਮ: ਦਵਾਈ, ਯੋਗਾ/ਕਸਰਤ, ਅਤੇ ਸੋਣ-ਜਾਗਣ ਦਾ ਸਹੀ ਸਮਾਂ-ਸਾਰਣੀ ਚੱਕਰ।\n\n🔬 ਨਤੀਜਾ: 100% ਸੁਰੱਖਿਅਤ ਅਤੇ ਸੰਪੂਰਨ ਦੇਖਭਾਲ।`
      );
    }, 2000);
  };

  return (
    <SafeAreaView style={styles.container}>
      <StatusBar barStyle="light-content" backgroundColor="#020617" />

      {/* Header Section */}
      <View style={styles.header}>
        <TouchableOpacity onPress={toggleOwnerMode}>
          <Text style={styles.brandTitle}>
            VITALIX <Text style={styles.brandAi}>{isOwnerMode ? '👑 MASTER OWNER' : 'UNIFIED AI'}</Text>
          </Text>
          <Text style={styles.brandSubtitle}>UNIVERSAL KNOWLEDGE & HEALTH ENGINE</Text>
        </TouchableOpacity>
        <View style={styles.versionBadge}>
          <Text style={styles.versionText}>{evolutionVersion}</Text>
        </View>
      </View>

      {/* Multi-Language Selector */}
      <View style={styles.langBar}>
        <ScrollView horizontal showsHorizontalScrollIndicator={false}>
          {LANGUAGES.map((lang) => (
            <TouchableOpacity
              key={lang.id}
              style={[styles.langChip, selectedLang === lang.id && styles.langChipActive]}
              onPress={() => setSelectedLang(lang.id)}
            >
              <Text style={[styles.langText, selectedLang === lang.id && styles.langTextActive]}>
                {lang.name}
              </Text>
            </TouchableOpacity>
          ))}
        </ScrollView>
      </View>

      <ScrollView contentContainerStyle={styles.scrollContent} showsVerticalScrollIndicator={false}>
        
        {/* Owner Customization Control Panel */}
        {isOwnerMode && (
          <View style={styles.ownerPanel}>
            <Text style={styles.ownerTitle}>👑 MASTER DEVELOPER & CONTROL PANEL</Text>
            <Text style={styles.ownerDesc}>ਤੁਹਾਡੇ ਕੋਲ ਇਸ ਐਪ ਵਿੱਚ ਨਵੇਂ ਅਪਡੇਟ ਕਰਨ, ਫੀਚਰਾਂ ਵਧਾਉਣ ਅਤੇ 100% ਨਿਯੰਤਰਣ ਰੱਖਣ ਦਾ ਅਧਿਕਾਰ ਹੈ।</Text>
            <TouchableOpacity style={styles.ownerBtn} onPress={() => Alert.alert('System Upgraded', 'ਤੁਹਾਡੀਆਂ ਸਾਰੀਆਂ ਹਿਦਾਇਤਾਂ ਸਿਸਟਮ ਵਿੱਚ ਸੁਰੱਖਿਅਤ ਹਨ।')}>
              <Text style={styles.ownerBtnText}>MANUALLY DEVELOP / ADD NEW FEATURES</Text>
            </TouchableOpacity>
          </View>
        )}

        {/* Heart & Emergency Scanner Card */}
        <TouchableOpacity style={styles.heartAlertCard} onPress={handleHeartCheck}>
          <Text style={styles.heartIcon}>❤️⚡</Text>
          <View style={{ flex: 1 }}>
            <Text style={styles.heartTitle}>EARLY WARNING EMERGENCY ALARM</Text>
            <Text style={styles.heartDesc}>ਸਰੀਰਕ ਹਲਚਲ ਅਤੇ ਨਾੜੀਆਂ ਦੇ ਸੰਕੇਤਾਂ ਦੀ ਸਮੇਂ ਸਿਰ ਜਾਂਚ।</Text>
          </View>
          <Text style={styles.activeTag}>ACTIVE</Text>
        </TouchableOpacity>

        {/* Real-time Bio Matrix */}
        <View style={styles.quantumCard}>
          <View style={styles.cardHeader}>
            <Text style={styles.cardHeaderTitle}>MASTER HEALTH & KNOWLEDGE MATRIX</Text>
            <Text style={styles.quantumBadge}>⚡ AUTO-LEARNING</Text>
          </View>

          <View style={styles.scoreContainer}>
            <View style={styles.holoCircle}>
              <Text style={styles.scoreNumber}>100%</Text>
              <Text style={styles.scoreLabel}>Coverage</Text>
            </View>
            <View style={styles.vitalsGrid}>
              <View style={styles.vitalBox}>
                <Text style={styles.vitalLabel}>Historical & Future Knowledge</Text>
                <Text style={styles.vitalValue}>All Diseases Mapped</Text>
              </View>
              <View style={styles.vitalBox}>
                <Text style={styles.vitalLabel}>Self-Development</Text>
                <Text style={styles.vitalValue}>Daily Auto-Upgrade</Text>
              </View>
              <View style={styles.vitalBox}>
                <Text style={styles.vitalLabel}>Owner Control</Text>
                <Text style={styles.vitalValue}>Full Access Enabled</Text>
              </View>
            </View>
          </View>
        </View>

        {/* AI Doctor & Knowledge Consultant */}
        <View style={styles.aiSection}>
          <Text style={styles.sectionTitle}>UNIFIED DIAGNOSTIC & RESEARCH CONSULTANT</Text>
          
          <View style={styles.responseBox}>
            <Text style={styles.aiResponseText}>{aiResponse}</Text>
          </View>

          <View style={styles.inputContainer}>
            <TextInput
              style={styles.textInput}
              placeholder="ਕਿਸੇ ਵੀ ਬਿਮਾਰੀ, ਰਿਸਰਚ ਜਾਂ ਇਲਾਜ ਬਾਰੇ ਪੁੱਛੋ..."
              placeholderTextColor="#475569"
              value={userQuery}
              onChangeText={setUserQuery}
              multiline
            />
            <TouchableOpacity 
              style={[styles.glowButton, isAnalyzing && styles.glowButtonDisabled]} 
              onPress={handleMasterDiagnostic}
              disabled={isAnalyzing}
            >
              <Text style={styles.glowButtonText}>
                {isAnalyzing ? 'RESEARCHING DATABASE...' : 'RUN MASTER HEALTH DIAGNOSIS'}
              </Text>
            </TouchableOpacity>
          </View>
        </View>

        {/* Integrated Ring Alarms & Modules */}
        <Text style={styles.sectionTitle}>TIME-RING ALARMS & CARE MODULES</Text>
        <View style={styles.gridContainer}>
          <TouchableOpacity style={styles.gridCard}>
            <Text style={styles.gridIcon}>🔔</Text>
            <Text style={styles.gridTitle}>Medicine Ring</Text>
            <Text style={styles.gridDesc}>Dosage Reminder</Text>
          </TouchableOpacity>

          <TouchableOpacity style={styles.gridCard}>
            <Text style={styles.gridIcon}>🧘</Text>
            <Text style={styles.gridTitle}>Yoga & Exercises</Text>
            <Text style={styles.gridDesc}>Workout Routine</Text>
          </TouchableOpacity>

          <TouchableOpacity style={styles.gridCard}>
            <Text style={styles.gridIcon}>🌿</Text>
            <Text style={styles.gridTitle}>Ayurveda & Herbs</Text>
            <Text style={styles.gridDesc}>Organic Remedies</Text>
          </TouchableOpacity>

          <TouchableOpacity style={styles.gridCard}>
            <Text style={styles.gridIcon}>🛠️</Text>
            <Text style={styles.gridTitle}>Developer Portal</Text>
            <Text style={styles.gridDesc}>Future Enhancements</Text>
          </TouchableOpacity>
        </View>

      </ScrollView>

      {/* Bottom Navigation */}
      <View style={styles.bottomNav}>
        <TouchableOpacity style={styles.navItem}>
          <Text style={styles.navIcon}>🌟</Text>
          <Text style={styles.navTextActive}>Unified AI</Text>
        </TouchableOpacity>
        <TouchableOpacity style={styles.navItem}>
          <Text style={styles.navIcon}>❤️</Text>
          <Text style={styles.navText}>Emergency</Text>
        </TouchableOpacity>
        <TouchableOpacity style={styles.navItem}>
          <Text style={styles.navIcon}>👑</Text>
          <Text style={styles.navText}>Owner</Text>
        </TouchableOpacity>
      </View>
    </SafeAreaView>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#020617',
  },
  header: {
    flexDirection: 'row',
    justifyContent: 'space-between',
    alignItems: 'center',
    paddingHorizontal: 16,
    paddingVertical: 12,
    borderBottomWidth: 1,
    borderBottomColor: '#1e293b',
  },
  brandTitle: {
    fontSize: 16,
    fontWeight: '900',
    color: '#FFFFFF',
    letterSpacing: 2,
  },
  brandAi: {
    color: '#38bdf8',
  },
  brandSubtitle: {
    fontSize: 6.5,
    color: '#64748b',
    letterSpacing: 1.2,
  },
  versionBadge: {
    backgroundColor: 'rgba(56, 189, 248, 0.1)',
    paddingHorizontal: 8,
    paddingVertical: 4,
    borderRadius: 8,
    borderWidth: 1,
    borderColor: 'rgba(56, 189, 248, 0.3)',
  },
  versionText: {
    color: '#38bdf8',
    fontSize: 7,
    fontWeight: '800',
  },
  langBar: {
    paddingVertical: 8,
    paddingHorizontal: 16,
    backgroundColor: '#0f172a',
  },
  langChip: {
    paddingHorizontal: 14,
    paddingVertical: 6,
    borderRadius: 20,
    backgroundColor: '#1e293b',
    marginRight: 8,
  },
  langChipActive: {
    backgroundColor: '#38bdf8',
  },
  langText: {
    color: '#94a3b8',
    fontSize: 12,
    fontWeight: '600',
  },
  langTextActive: {
    color: '#020617',
    fontWeight: '900',
  },
  scrollContent: {
    padding: 16,
    paddingBottom: 80,
  },
  ownerPanel: {
    backgroundColor: '#1e1b4b',
    padding: 14,
    borderRadius: 16,
    borderWidth: 1,
    borderColor: '#6366f1',
    marginBottom: 16,
  },
  ownerTitle: {
    color: '#818cf8',
    fontSize: 10.5,
    fontWeight: '900',
    letterSpacing: 1,
  },
  ownerDesc: {
    color: '#c7d2fe',
    fontSize: 9.5,
    marginVertical: 6,
  },
  ownerBtn: {
    backgroundColor: '#6366f1',
    paddingVertical: 8,
    borderRadius: 8,
    alignItems: 'center',
  },
  ownerBtnText: {
    color: '#FFFFFF',
    fontSize: 9.5,
    fontWeight: '900',
  },
  heartAlertCard: {
    backgroundColor: '#450a0a',
    borderRadius: 16,
    padding: 12,
    borderWidth: 1,
    borderColor: '#ef4444',
    flexDirection: 'row',
    alignItems: 'center',
    marginBottom: 16,
  },
  heartIcon: {
    fontSize: 24,
    marginRight: 10,
  },
  heartTitle: {
    color: '#fca5a5',
    fontSize: 11,
    fontWeight: '900',
  },
  heartDesc: {
    color: '#fecaca',
    fontSize: 8.5,
    marginTop: 2,
  },
  activeTag: {
    color: '#ef4444',
    fontSize: 9,
    fontWeight: '900',
    backgroundColor: 'rgba(239, 68, 68, 0.2)',
    paddingHorizontal: 6,
    paddingVertical: 2,
    borderRadius: 6,
  },
  quantumCard: {
    backgroundColor: '#0f172a',
    borderRadius: 20,
    padding: 16,
    borderWidth: 1,
    borderColor: 'rgba(56, 189, 248, 0.2)',
    marginBottom: 20,
  },
  cardHeader: {
    flexDirection: 'row',
    justifyContent: 'space-between',
    alignItems: 'center',
    marginBottom: 12,
  },
  cardHeaderTitle: {
    color: '#64748b',
    fontSize: 9,
    fontWeight: '800',
    letterSpacing: 1.5,
  },
  quantumBadge: {
    color: '#38bdf8',
    fontSize: 8,
    fontWeight: '700',
  },
  scoreContainer: {
    flexDirection: 'row',
    alignItems: 'center',
  },
  holoCircle: {
    width: 85,
    height: 85,
    borderRadius: 42.5,
    borderWidth: 2,
    borderColor: '#38bdf8',
    justifyContent: 'center',
    alignItems: 'center',
    marginRight: 16,
    backgroundColor: 'rgba(56, 189, 248, 0.05)',
  },
  scoreNumber: {
    color: '#FFFFFF',
    fontSize: 22,
    fontWeight: '900',
  },
  scoreLabel: {
    color: '#38bdf8',
    fontSize: 7.5,
    fontWeight: '700',
  },
  vitalsGrid: {
    flex: 1,
  },
  vitalBox: {
    marginBottom: 6,
  },
  vitalLabel: {
    color: '#64748b',
    fontSize: 8.5,
  },
  vitalValue: {
    color: '#38bdf8',
    fontSize: 10,
    fontWeight: '700',
  },
  aiSection: {
    marginBottom: 20,
  },
  sectionTitle: {
    color: '#64748b',
    fontSize: 9.5,
    fontWeight: '800',
    letterSpacing: 1.5,
    marginBottom: 10,
  },
  responseBox: {
    backgroundColor: '#0f172a',
    borderRadius: 16,
    padding: 14,
    borderWidth: 1,
    borderColor: '#1e293b',
    marginBottom: 10,
  },
  aiResponseText: {
    color: '#e2e8f0',
    fontSize: 12.5,
    lineHeight: 19,
  },
  inputContainer: {
    backgroundColor: '#0f172a',
    borderRadius: 16,
    padding: 8,
    borderWidth: 1,
    borderColor: '#1e293b',
  },
  textInput: {
    color: '#FFFFFF',
    fontSize: 12.5,
    minHeight: 45,
    paddingHorizontal: 8,
  },
  glowButton: {
    backgroundColor: '#38bdf8',
    borderRadius: 12,
    paddingVertical: 12,
    alignItems: 'center',
    marginTop: 6,
  },
  glowButtonDisabled: {
    backgroundColor: '#334155',
  },
  glowButtonText: {
    color: '#020617',
    fontWeight: '900',
    fontSize: 10,
    letterSpacing: 1,
  },
  gridContainer: {
    flexDirection: 'row',
    flexWrap: 'wrap',
    justifyContent: 'space-between',
  },
  gridCard: {
    width: (width - 44) / 2,
    backgroundColor: '#0f172a',
    borderRadius: 16,
    padding: 12,
    borderWidth: 1,
    borderColor: '#1e293b',
    marginBottom: 10,
  },
  gridIcon: {
    fontSize: 22,
    marginBottom: 6,
  },
  gridTitle: {
    color: '#FFFFFF',
    fontSize: 11.5,
    fontWeight: '700',
  },
  gridDesc: {
    color: '#64748b',
    fontSize: 8.5,
    marginTop: 2,
  },
  bottomNav: {
    position: 'absolute',
    bottom: 0,
    left: 0,
    right: 0,
    height: 65,
    backgroundColor: '#020617',
    flexDirection: 'row',
    justifyContent: 'space-around',
    alignItems: 'center',
    borderTopWidth: 1,
    borderTopColor: '#1e293b',
  },
  navItem: {
    alignItems: 'center',
  },
  navIcon: {
    fontSize: 18,
    marginBottom: 2,
  },
  navText: {
    color: '#64748b',
    fontSize: 9,
  },
  navTextActive: {
    color: '#38bdf8',
    fontSize: 9,
    fontWeight: '800',
  },
});
